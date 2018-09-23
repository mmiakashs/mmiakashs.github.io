---
layout: post
title: Introduction to Kaggle API in Google Colab (Part-I)
comments: true
---

This introductory article helps to prepare the google colab to use the kaggle api. Moreover, we will cover a couple of usages of kaggle-api, most importantly import data from kaggle. So let's begin...

At first, create a jupyter notebook in the google colab and change the runtime to python3. After that follow the following simple steps to prepare the google colab to use Kaggle-API.

## Prepare Google Colab for Kaggle-API

Install the Kaggle library in google colab instance.
```
!pip3 install kaggle
```

## Kaggele API Authentication

We need to enable kaggle api authentication and the auth token file to interact with the kaggle api system. Follow the following steps to get the authentication:

*   Create an account or login in [kaggle.com](https://www.kaggle.com)
*   After that go to My Account and click **Create New API Token**, which will download kaggle.json
*   Upload the kaggle.json file into any folder of google drive



## Google drive authentication
In this step, we will retrieve the google drive authentication to use drive files(in this tutorial we will need this authentication to retrieve the kaggle.json file, which we uploaded in the previous steps). Open the authentication link, which you will get in the output, after executing the following code cell. Then copy the authentication code into the cell output's input box and complete the authentication process.


```
from googleapiclient.discovery import builds
import io, os
from googleapiclient.http import MediaIoBaseDownload
from google.colab import auth

auth.authenticate_user()
```

Search the kaggle.json file from google drive and copied into ```~/.kaggle/kaggle.json```


```
drive_service = build('drive', 'v3')
results = drive_service.files().list(
        q="name = 'kaggle.json'", fields="files(id)").execute()
kaggle_api_key = results.get('files', [])

filename = "/content/.kaggle/kaggle.json"
os.makedirs(os.path.dirname(filename), exist_ok=True)

request = drive_service.files().get_media(fileId=kaggle_api_key[0]['id'])
fh = io.FileIO(filename, 'wb')
downloader = MediaIoBaseDownload(fh, request)
done = False
while done is False:
    status, done = downloader.next_chunk()
    print("Download %d%%." % int(status.progress() * 100))
os.chmod(filename, 600)

```
In the google colab, the kaggle.json file needs to stored in the ~/kaggle directory. That's why we need to copy the kaggle.json file into ~/.kaggle directory
```
!mkdir ~/.kaggle
!cp /content/.kaggle/kaggle.json ~/.kaggle/kaggle.json
```

Execute the following command to verify whether the kaggle.json is stored in the appropriate location: **~/.kaggle/kaggle.json**


```
ls ~/.kaggle
```
If the output of this command shows the kaggle.json file then we are ready to use the kaggle-cli API. The details of kaggle-cli are given [here](https://github.com/floydwch/kaggle-cli)

## Sample usages of kaggle-cli

### Retrieve Kaggle Competitions List


```
!kaggle competitions list
```

    ref                                              deadline             category            reward  teamCount  userHasEntered
    -----------------------------------------------  -------------------  ---------------  ---------  ---------  --------------
    digit-recognizer                                 2030-01-01 00:00:00  Getting Started  Knowledge       2492           False
    titanic                                          2030-01-01 00:00:00  Getting Started  Knowledge       9736           False
    house-prices-advanced-regression-techniques      2030-01-01 00:00:00  Getting Started  Knowledge       4169           False
    imagenet-object-localization-challenge           2029-12-31 07:00:00  Research         Knowledge         25           False
    competitive-data-science-predict-future-sales    2019-01-01 23:59:00  Playground           Kudos       1440           False
    ga-customer-revenue-prediction                   2018-11-15 23:59:00  Featured           $45,000        792            True
    inclusive-images-challenge                       2018-11-05 23:59:00  Research           $25,000        264           False
    rsna-pneumonia-detection-challenge               2018-10-24 23:59:00  Featured           $30,000        877            True
    tgs-salt-identification-challenge                2018-10-19 23:59:00  Featured          $100,000       2647            True
    airbus-ship-detection                            2018-10-04 23:59:00  Featured           $60,000        835           False
    new-york-city-taxi-fare-prediction               2018-09-25 23:59:00  Playground       Knowledge       1075           False
    forest-cover-type-kernels-only                   2018-09-24 23:59:00  Playground       Knowledge        335           False
    demand-forecasting-kernels-only                  2018-09-24 23:59:00  Playground       Knowledge        427           False
    whats-cooking-kernels-only                       2018-09-24 23:59:00  Playground       Knowledge        492           False
    flavours-of-physics-kernels-only                 2018-09-24 23:59:00  Playground       Knowledge         56           False
    movie-review-sentiment-analysis-kernels-only     2018-09-24 23:59:00  Playground       Knowledge        377           False
    costa-rican-household-poverty-prediction         2018-09-19 23:59:00  Playground            Swag        619           False
    google-ai-open-images-object-detection-track     2018-08-30 23:59:00  Featured           $30,000        454           False
    google-ai-open-images-visual-relationship-track  2018-08-30 23:59:00  Featured           $20,000        232           False
    home-credit-default-risk                         2018-08-29 23:59:00  Featured           $70,000       7198           False


### List Data Files in a Kaggle Competition


```
# -c: competition name
!kaggle competitions files -c planet-understanding-the-amazon-from-space
```

    name                              size  creationDate
    -------------------------------  -----  -------------------
    train-jpg.tar.7z                 600MB  2017-04-20 00:13:50
    test-jpg.tar.7z                  603MB  2017-04-20 00:15:13
    train-tif-v2.tar.7z               13GB  2017-05-06 06:13:24
    test-tif-v2.tar.7z                19GB  2017-05-06 06:27:29
    test-jpg-additional.tar.7z       304MB  2017-05-06 06:49:41
    Kaggle-planet-test-tif.torrent     2MB  2017-05-06 06:54:37
    Kaggle-planet-train-tif.torrent    1MB  2017-05-06 06:54:55
    sample_submission_v2.csv.zip     154KB  2017-05-09 03:01:24
    train_v2.csv.zip                 159KB  2017-05-09 03:01:24
    test_v2_file_mapping.csv.zip     110KB  2017-06-08 00:26:28


#### Show the leaderboard of a kaggle competitions


```
!kaggle competitions leaderboard planet-understanding-the-amazon-from-space -s
```

    teamId  teamName                         submissionDate       score
    ------  -------------------------------  -------------------  -------
    764901  SYSU CISLab                      2017-07-20 23:32:25  0.93448
    776206  Russian Bears                    2017-07-20 23:34:32  0.93448
    623630  Urucu                            2017-07-20 23:41:07  0.93443
    623281  Plant                            2017-07-20 19:19:22  0.93431
    647582  Team samogon                     2017-07-20 08:47:56  0.93422
    744470  Clear Sky                        2017-07-20 19:51:39  0.93419
    626431  Kyle                             2017-07-20 15:26:36  0.93412
    741719  ods.ai                           2017-07-20 23:46:33  0.93408
    624465  bestfitting                      2017-07-20 23:48:39  0.93398
    623172  deepsense.io                     2017-07-20 13:22:36  0.93392
    624135  Moss                             2017-07-20 23:22:18  0.93386
    757613  Daniel FG                        2017-07-20 23:56:03  0.93381
    654347  🌴team-amazon-forest🌴             2017-07-20 08:21:17  0.93353
    728947  CVFakers                         2017-07-20 23:05:50  0.93351
    623222  dhammack                         2017-07-20 21:52:14  0.93349
    783137  Eduardo Franco                   2017-07-20 19:42:02  0.93342
    625451  YunYang                          2017-07-17 11:47:49  0.93342
    ...


### Download Kaggle Competition Leaderboard


```
!kaggle competitions leaderboard planet-understanding-the-amazon-from-space -d
```


### Download Dataset from Kaggle Competitions

In this article, we will download data from [Planet: Understanding the Amazon from Space](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space)

Please note that you must accept the terms and condition of that kaggle competitions to download data from any kaggle competition.


```
!mkdir ~/data
!cd ~/data
!mkdir planet
!cd planet
```


```
# -c: competition name
# -f: which file you want to download
# -p: path to where the file should be saved
!kaggle competitions download -c planet-understanding-the-amazon-from-space -f train-jpg.tar.7z -p ~/data/planet/
!kaggle competitions download -c planet-understanding-the-amazon-from-space -f test-jpg.tar.7z -p ~/data/planet/
!kaggle competitions download -c planet-understanding-the-amazon-from-space -f train_v2.csv.zip -p ~/data/planet/
```

#### Extract the datafiles


Install 7zip to extract the datafiles
```
!apt-get install p7zip-full
```

```
# Unzip the 7zip files
# -d: which file to un7zip
!p7zip -d ~/data/planet/test-jpg.tar.7z
!p7zip -d ~/data/planet/train-jpg.tar.7z
```

```
# Unzip the .tar files
!tabr -xvf ~/data/planet/test-jpg.tar
!tar -xvf ~/data/planet/train-jpg.tar
```

```
!unzip ~/data/planet/train_v2.csv.zip -d ~/data/planet/
```

```
ls
```

    adc.json  planet/  sample_data/  test-jpg.tar  train-jpg.tar


In the first part of this kaggle API tutorial, we covered the basic usage of this API. In the next part, we will cover the advanced usages of kaggle API, such as submit a solution to a kaggle competition. Till then you can see the documentation of [kaggle-cli](The details of kaggle-cli is given [here](https://github.com/floydwch/kaggle-cli) and try the different usage of kaggle-cli.

I write this tutorial by following a tutorial of Cory Kendrick on [fastai course notebook](https://github.com/corykendrick/fastai_in_colab), so a big thanks to [Cory  Kendrick](https://github.com/corykendrick).

### If you have any comments or feedback regarding this articles or my writings, please don't hesitate to share with me.

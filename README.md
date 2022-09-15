# drive-to-yt

First of all let us understand what are we trying to achieve and how are we going to proceed for that? We have some files on drive and want to
upload it on _yt. Simple solution is that we download them and then upload directly upload them with _yt studio. But what if the data is 100s
of GigaBytes and 1000s of files. In principle you can do this whatever is the size of the data provided you are given an infinite time and 
infinte bandwidth. There is an faster, optimal but not so easy method to achieve this. We will discuss this intricate process here.

## What is the Solution

We will make an app that can access _yt data and also edit that. I mean everything that we can do with _yt Studio we can do that with this app also. 

**What if** *we can run this app on google collab*, keep in mind that we can access, modify, delete drive files with google collab easily.

If we do so on google collab then we have many advantages
* We do not need to download the data, inturn saving 100s of Gigs.
* Uploading will be handelled on google server, means a lot lot faster.
* Scripting allows us to make consistent upload, I means more systematic.
* *We learn a lot more about the web mess, how intricate and dangerous it is.*

Now we discuss step by step how this is done....


## Google Develpoer Console

Visit https://console.cloud.google.com to learn more about google developer console.

### Managing resources

Do modify, delete, create new projects go to 
https://console.cloud.google.com/cloud-resource-manager

### Create A Project 

1. `Create Project` > Fill out `Project name` > `CREATE`.
2. Select the project and go to `APIs & Services` > `Enabled APIs & servies`
3. `+ ENABLE APIS AND SERVICES` and serach for `youtube data api v3` and select and enable it. This will configure our project to handle request related to `youtube data`.
4. `APIs & Services` > `OAuth consent screen` > `External` > `CREATE`
5. Fill out `App name` and `User support email` and `Developer contact information`. Any name will be okay.
6. `SAVE AND CONTINUE...` > > `Test users` > `ADD USERS`(Add your email address herer) > `SAVE AND CONINUE`. This will add you as a test user.
7. Now go to `Credentials` > `+ CREATE CREDENTIALS` > `OAuth client ID`.
8. Select `Application type` to `Desktop app` and give some name. and `CREATE`.
9. Now your `Client ID` and `Client Secret` will be visible to your screen. Copy them. They will be required later.
10 Now open `DRIVE-to-YT` file in google collab and follow the notebook instructions. and your drive files are ready to be uploaded on youtube.



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

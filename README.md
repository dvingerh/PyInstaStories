# PyInstaStories
Python script to download Instagram stories from a single user or multiple users at once. Supports Python 2.7 and 3.5.


# How to use

Make sure you have the following dependency installed: https://github.com/ping/instagram_private_api


### Arguments

The `--username` and `--password` arguments are required to generate a new cookie file or when an existing cookie file has expired. You can omit these two arguments if there is a working login cookie file available already.

`--download` — User(s) to download. Multiple users must be seperated by a space.

`--batch-file` — Download stories from usernames in a text file.

`--taken-at` — PyInstaStories will save files with a datetime format: `2019-01-07_22-51-43.jpg`

`--no-thumbs` — PyInstaStories will skip downloadable video story thumbnail images.

`--hq-videos` — PyInstaStories will download slightly higher quality video stories. Requires `ffmpeg`. Not stable right now.

### Examples

Download stories of 3 users.  
`python3 pyinstastories.py -d jacobsartorius justinbieber lilhankwilliams`

Download stories of 1 user. Save files with a datetime format and skip downloading of video thumbnail images.  
`python3 pyinstastories.py -d iamcardib --taken-at --no-thumbs`

Download stories from a text file. Pass login username and password as arguments.  
`python3 pyinstastories.py --batch-file usernames.txt --username johndoe --password grapefruits`

##### Example terminal output

```
$ python3 pyinstastories.py --download justinbieber
----------------------------------------------------------------------
[I] PYINSTASTORIES (SCRIPT V2.1 - PYTHON V3.7.3) - 05:55:42 PM
----------------------------------------------------------------------
[I] Using cached login cookie for "johndoe".
[I] Login to "johndoe" OK!
[I] Login cookie expiry date: 2019-08-07 at 09:54:43 PM
----------------------------------------------------------------------
[I] Files will be downloaded to C:\Users\User\Documents\Git\PyInstaStories
----------------------------------------------------------------------
[I] Getting stories for: justinbieber
----------------------------------------------------------------------
[I] Downloading video stories. (7 stories detected)
----------------------------------------------------------------------
[I] (1/7) Downloading video: 41107421_150110362713394_6909049832863331499_n.mp4
[I] (2/7) Downloading video: 40704767_352431668802214_7535329190798115834_n.mp4
[I] (3/7) Downloading video: 32675407_899984993677896_5838612576283769538_n.mp4
[I] (4/7) Downloading video: 27460743_1232788393557486_4163271676685655927_n.mp4
[I] (5/7) Downloading video: 40991261_591854457989117_3573059593419810351_n.mp4
[I] (6/7) Downloading video: 27449739_373199263333116_2195630862018446526_n.mp4
[I] (7/7) Downloading video: 32786476_689302061513389_6323122299924594750_n.mp4
----------------------------------------------------------------------
[I] Downloading image stories. (3 stories detected)
----------------------------------------------------------------------
[I] (1/3) Downloading image: 61787819_1607274159404970_4836984492900662152_n.jpg
[I] (2/3) Downloading image: 64505667_498208200986305_7034972402491620659_n.jpg
[I] (3/3) Downloading image: 64264791_1350148401799309_7365462912390446749_n.jpg
----------------------------------------------------------------------
[I] Story downloading ended with 3 new images and 7 new videos downloaded.
----------------------------------------------------------------------
```

# PyInstaStories
CLI script to download Instagram stories from a single user or multiple users at once. Supports Python 2.7 and 3.5.


# How to use

Make sure you have the following dependency installed: https://github.com/ping/instagram_private_api

Available arguments are `--username`, `--password` and `--download`, but you can omit `--username`, `--password` if there is a login cookie file available already.

The `--download` argument supports multiple users, each user is seperated by a space.

Example: `python3 pyinstastories.py -d jacobsartorius justinbieber lilhankwilliams`

### Example

```
> python3 pyinstastories.py -d jordynjones
----------------------------------------------------------------------
PYINSTASTORIES (SCRIPT V1.4 - PYTHON V3.6.3) - 01:16:38 AM
----------------------------------------------------------------------
[I] Using cached login cookie for "johndoe".
[I] Login to "johndoe" OK!
[I] Login cookie expiry date: 2018-08-18 at 04:40:56 PM
----------------------------------------------------------------------
[I] Files will be downloaded to C:\Users\User\Documents\Git\PyInstaStories
----------------------------------------------------------------------
[I] Getting stories for user: jordynjones
----------------------------------------------------------------------
[I] Downloading video: 37813815_215083095840615_4630133302956493383_n.mp4
[I] Downloading image: 38066226_439347253244259_7841321044982890496_n.jpg
[I] Downloading image: 38541931_272408410204408_6934439177173860352_n.jpg
[I] Downloading image: 38166262_230879184287581_2338295584533774336_n.jpg
[I] Downloading image: 38752915_246521029518941_7519825270950330368_n.jpg
[I] Downloading image: 38052809_2182358915374391_4548264508405055488_n.jpg
[I] Downloading image: 38080828_530212454075962_3213326425847234560_n.jpg
----------------------------------------------------------------------
[I] Story downloading ended with 6 new images and 1 new videos downloaded.
----------------------------------------------------------------------
```

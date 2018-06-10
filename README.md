# PyInstaStories
CLI script to download Instagram stories from a given user. Supports Python 2.7 and 3.5.


# How to use

Make sure you have the following dependency installed: https://github.com/ping/instagram_private_api

Available arguments are `--username`, `--password` and `--download`, but you can omit `--username`, `--password` if there is a login cookie file available already.

### Example

```
> python3 pyinstastories.py -d "jacobsartorius"
----------------------------------------------------------------------
PYINSTASTORIES (SCRIPT V1.2 - PYTHON V3.6.3) - 07:46:43 PM
----------------------------------------------------------------------
[I] Using cached login cookie for "johndoe".
[I] Login to "johndoe" OK!
[I] Login cookie expiry date: 2018-05-27 at 04:40:56 PM
--------------------------------------------------
Getting stories for user 'jacobsartorius' ...
--------------------------------------------------
[I] Downloading video into C:\Users\User\Desktop\stories/stories/jacobsartorius/32275618_1651418691639843_511834982014950862_n.mp4
[I] Downloading video into C:\Users\User\Desktop\stories/stories/jacobsartorius/32517291_189849734891972_4663753825336221593_n.mp4
[I] Downloading video into C:\Users\User\Desktop\stories/stories/jacobsartorius/32655179_2207753162587548_6278569131428248597_n.mp4
[I] Downloading video into C:\Users\User\Desktop\stories/stories/jacobsartorius/32077783_2038028266523708_6160051017498413051_n.mp4
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/32203303_219425121987636_9162122599168212992_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/31680625_198319374134675_4153861316630544384_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/31694915_109540646593804_7825875401988636672_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/31888449_858885097632840_6208524751359442944_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/32377364_1784230578311096_1660142371871916032_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/32078859_381414955677912_3314394217572204544_n.jpg
[I] Downloading image into C:\Users\User\Desktop\stories/stories/jacobsartorius/32362287_637168276623962_5935568322589360128_n.jpg
--------------------------------------------------
[I] Story downloading ended with 7 new images and 4 new videos downloaded.
--------------------------------------------------
```

# e621_collector



## 0.01b (2019-08-23)
 <br> <b>initial release</b>
1. tags were inputted separated by space(' ')
2. tags re-typing(modifying) were not supported


## 0.01.1b (2019-08-24)
<br> <b>fast patch</b>
1. tags now separated by commma(',) and tags that have space between words <br>(e.g, big breasts) is now supported ( 0.01b taked it as 'big' and 'breasts')
2. tags re-typing ( + only, - only, both) is now supported


## 0.02b <br>
<del><b>expecting 2019-08-25 </b></del>  --><b> released at 2019-08-24 as version 0.02.1b</b>
1. (error) images were downloaded as "sample", not original resolution <br> change parsing download link (not sample)

## 0.02.1b <br>
<b>fast patch</b>
1. releas again at the same day (2019-08-24) with fixing error

## 0.03b <br>
<b>Aysnc : aiohttp, asyncio added</b><br>
1. spead increasement about 5~8 times by 0.02.1b

## 0.04b <br>
1. Fixed bug when searching tag with '/' e.g) female/male
2. supporting filter downloading only image/videos, but still don't support swf.(flash)
3. Made custom search
   (1). searching tag(+) and tag(or)
   (2). filter posts with tag(-)
   (3). filter points and favpoint range
   (4). filter file type
4. Added input() before every sys.exit(-1) to make sure to the users

## 0.04.1b (2019-09-02)<br>
<b>fast patch</b><br>
<b>Emergency Patch Fixing NoneAttribute Error</b>

1. decreased sleep time 3 to 1 second
   --> async.sleep() for every post is enough
   
<del>## 2019-09-12 Migrating to Java</del>

<del>1. To make every OS handy</del>


## 0.04.2b (2019-09-14)<br>
<b>Minor Bug Patch</b><br>
1. Fixed : Error appeared when tag includes "/f" e.g) male/female
2. Fixed : Not proper program exit when htis maximum download
3. Fixed : Error that when searched for only explicit, it returned all rating posts
4. Added option to shutdown computer after downloading

<br>(2019-09-21)
1. Fixed search_filter ">=" to ">"<br>
there will be downloading all 75 posts in a page unless there are over 6 search queries<br>
(some posts where skipped when fav_count:>=60, post with fav_count 60 was filtered)

2. parsing for static url of post (original post url) is changed more preciselly<br>
in case of comment using big titles ('h4')

## 0.05 (2019-09-23)<br>
<b>A step for UI<b><br>
 1. Changed fetch static url method to async by pairing 10 posts at once, which made slightly fast
 2. Removed printing urls when downloading
 3. simplfied CLI by showing spinnner, acknowledging progress (This is necessary for UI job later)
 

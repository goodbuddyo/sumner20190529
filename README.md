# README
# sumner20190529
# Assignment: Make the bottom row 2-col and Add images that resize to 5 remaining media-box areas.

Hi Lisa,

Here's a rundown on the updates:



1 - remove the last &lt;div class="four columns"> ... &lt;/div>

2 - change the other 2 divs in that row to "six columns" and  nest another row div  under the h2 containing a five col div (for the image)  and a seven col div (for the text)

3 - copy the &lt;p style="padding:20px 0 0 0;" class="center">&lt;mg>...&lt;/p> from the top hero area and paste below each of the lower 5 media-box &lt;h2> tags

4 - update the 5 media-box image refs
  Erin-Weiss.jpg
  Samantha-Hoffert.jpg
  Caleigh-Ward.jpg
  teven-Vournazos.jpg
  Allison-Holden.jpg

5 - for semantics update the 5 lower  &lt;p> tags images from 
&lt;p style="padding:20px 0 0 0;" class="center">...&lt;/p>
to
&lt;figure style="padding:20px 36px 0 36px;"  class="center">...&lt;/figure>
and add 
&lt;figcaption> 
tags to credit the artists
(may want to check for permission to display the art )
(may also want to update the top Hero image &lt;p> tag to &lt;figure> for consistency )

6 - Add a class to the media-box &lt;H2> tags to make them stand out more
 &lt;h2 class="text21">5 Easy Steps&lt;/h2>

 7 - Since 2 col media-boxes needs some different styling than the 3 col media boxes,  
  add a new style to main.css (or in a local &lt;style> tag until this gets approved for main.css)

--------------------------

Some minor tweaks: 
the padding-bottom of the media-boxes seems a little tight.
I added 8 pixels with an inline &lt;style> tag

.media-box-content { padding: 20px 12px 18px 12px; }

Also, using display: flex should make all the media-boxes the same height
  
.tb-padding-10 { display:flex; flex-wrap:wrap; }
.tb-padding-10 .columns { display:flex;  }
.media-content-box {display:flex; }


-------------------------------

That should do it. 
The only style changes needed are in step 7 & 8 and the inline style change in step 5. 

---------------------------



As a side note, this page showed a 404 error and a Depracated warning in the console, which also appears on the live site: https://byonewtown.org/

The 404 can be addressed by adding a favicon.ico file to the images folder (for some reason they reference a .png file)

The warning involves a recent XMLHttpRequest2 spec change. 
Here are a few related comments:

https://developers.google.com/web/updates/2012/01/Getting-Rid-of-Synchronous-XHRs
https://x443.wordpress.com/2012/12/01/why-you-should-use-xmlhttprequest-asynchronously/
https://github.com/jquery/jquery/issues/3975
http://www.codecheese.com/2017/03/fix-synchronous-xmlhttprequest-on-the-main-thread-is-deprecated/



I'll check in with you tomorrow, or please call or email me if you have any questions or concerns. 

Thanks!
Sean O'
203 561 5797



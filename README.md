# README
# sumner20190529
# Assignment: Make the bottom row 2-col and Add images that resize to 5 remaining media-box areas.

Hi Lisa,

Here's a rundown on the updates:

1 - remove the last <div class="four columns"> ... </div>

2 - change the other 2 divs in that row to "six columns"

3 - copy the <p style="padding:20px 0 0 0;" class="center"><img>...</p> from the top hero area and paste below each of the lower 5 media-box <h2> tags

4 - update the 5 media-box image refs
  Erin-Weiss.jpg
  Samantha-Hoffert.jpg
  Caleigh-Ward.jpg
  teven-Vournazos.jpg
  Allison-Holden.jpg

5 - for semantics update the 5 lower  <p> tags images from 
<p style="padding:20px 0 0 0;" class="center">...</p>
to
<figure style="padding:10px 20px 0 20px;" class="center">.</figure>
and add 
<figcaption> 
tags to credit the artists
(may want to check for permission to display the art )
(may also want to update the top Hero image <p> tag to <figure> for consistency )

6 - Add a class to the media-box <H2> tags to make them stand out more
 <h2 class="text21">5 Easy Steps</h2>

 7 - Since the added width of the bottom two media-boxes makes the <p> text look odd, increase the left and right padding of the media boxes - add a media-box-2col class to those two boxes 
 <div class="media-box-content media-box-2col">

 and add a new style to main.css (or in a local <style> tag until this gets approved for main.css)

  .media-box-content.media-box-2col {
    padding: 20px 22px 12px 22px;
  }

8 -  In the media query for mobile, make the padding for these bottom two media-boxes match the padding of the other 3, 

  /* Smaller than mobile */
  @media (max-width: 550px) {
    .mobile-center {text-align:center;}
    
    .media-box-content.media-box-2col {
      padding: 20px 12px 12px 12px;
    }
  }
--------------------------


Some minor tweaks: 
the padding-bottom of the media-boxes seems a little tight.
I added 8 pixels with an inline <style> tag

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



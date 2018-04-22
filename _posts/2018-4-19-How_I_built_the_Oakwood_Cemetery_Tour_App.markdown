---
layout: post
comments: true
title:  "How I built the Oakwood Cemetery Tour App"
date:   2018-4-19 Maps 11:11:11 +0100
thumbnail: earth.jpg
---
How I built the Oakwood Cemetery Tour App. 
I first became interested in Oakwood Cemetery when I saw a flyer for a Historic tour conducted by the Organization. Save Austin’s Cemeteries (SAC) for a historic tour of Oakwood Cemetery. So I decided to build a ESRI Web App that someone could use to find individual graves they would probably include on the tour
1.	I overlaid the lot maps I found for Oakwood using Google Earth – Image Overlay function. (I find this easier to use than ArcGIS’ rubbersheet function). I found the maps on the Austin Genealogical Website here: http://www.austintxgensoc.org/cemeteries/oakwood-cemetery/ I did this to get lat/longs for each lot. 
 
2.	Once I overlaid the maps I added a center point for each cemetery lot (as opposed to each grave). I numbered each point according to lot number. This was more time consuming than needed to be as I could have just numbered the lots according the ones I wanted to include on the tour but I would like to maybe try to build a map app to look up anyone in the cemetery at a later date since all the names and lots are listed here. http://www.austintxgensoc.org/cemeteries/oakwood-cemetery/oakwood-cemetery-list-of-graves-old/ 


For the time being I only wanted to list only the more historic personages that I have found mentioned in a couple different publications to use for a tour web app (these are the ones shown in the red tear drop markers) but I now have them if I want to include all the names later on. I saved the KML and then converted it to a CSV for import into ArcGIS Online Map tour. I didn’t exactly use these directions but these are close enough to use to do the same thing: https://www.esri.com/arcgis-blog/products/arcgis-enterprise/uncategorized/create-a-story-map-tour-using-a-spreadsheet/ 
The important thing is I matched the name from the graves list, with their lot number and the lat/log from Google Earth and put them all in a CSV with the right column names for the ArcGIS map tour import (see link above).
Note: To avoid any copy write issues I used existing links and pics from Wikipedia for most of the text (and a couple of similar public sites). All the pics are included from URL links as opposed to being stored anywhere. Here is the edit screen. All sources are referenced in the app.
  

After that I just saved it and made sure it was shared (as well as the web map) and published it here: 


{% if page.comments %} 
<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://http-esri4apl-site.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
{% endif %}

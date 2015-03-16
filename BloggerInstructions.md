# Introduction #

Adding this script to your blog is extremely simple, just follow the instructions below.


# Version 3.0 #

Copy and paste this code into an HTML / JavaScript widget:

```
<script src="http://blogidol-greetbox.googlecode.com/files/bi-TextToBeDisplayedDiv-minv3.0.js"
type="text/javascript">
</script>
<div id="mainDisplayDiv" style="background:#F8F8FF;border:1px solid #B6AFA9;display:none">
<div style="float: right; margin-right: 5px; margin-top: 5px;">
<href a="#" onclick="closeGreetBox('7')"><img border="0" alt="x" 
src="http://img214.imageshack.us/img214/9837/closebutton.gif" />
</href></div>
<div id="dynamicContentDisplayed">
</div>
<script type="text/javascript">
// Give your feed url here
var feedURL = "http://feeds2.feedburner.com/blogidol";
var dynamicHTMLText = displayRequiredText(feedURL);
document.getElementById("dynamicContentDisplayed").innerHTML = dynamicHTMLText;
</script>
</div>
<script src="http://blogidol-greetbox.googlecode.com/files/HideShowDivV3.0.js"
type="text/javascript">
</script>
<script type="text/javascript">
showHideDiv();
</script>
```

Before saving, change http://feeds2.feedburner.com/blogidol above with your own feed URL.

Starting with version 3.1 I implemented a system that works only with Blogger blogs. Instead of your feed URL you enter your blog URL, without a trailing backslash, e.g. "http://yourblog.blogspot.com". This allows the welcome message to also display an invitation to view your /view version. For this to work, you have to enable full feeds (for /view) and also redirect feeds from /feed/default to the feedburner feed (if that's what you're using).

# Version 3.1+ #
```
<script src="http://blogidol-greetbox.googlecode.com/files/bi-TextToBeDisplayedDiv-minv3.1.js" type="text/javascript"></script>
<div id="mainDisplayDiv" style="background:#F8F8FF;border:1px solid #B6AFA9;display:none">
<div style="float: right; margin-right: 5px; margin-top: 5px;">
<href a="#" onclick="closeGreetBox('7')"><img border="0" alt="x" src="http://img214.imageshack.us/img214/9837/closebutton.gif" />
</href></div>
<div id="dynamicContentDisplayed">
</div>
<script type="text/javascript">
// Give your feed url here
var feedURL = "http://3w.blogidol.ro";var dynamicHTMLText = displayRequiredText(feedURL);
document.getElementById("dynamicContentDisplayed").innerHTML = dynamicHTMLText;
</script>
</div>
<script src="http://blogidol-greetbox.googlecode.com/files/HideShowDivV3.0.js" type="text/javascript">
</script>
<script type="text/javascript">
showHideDiv();
</script>
```

Before saving, change http://3w.blogidol.ro above with your own blog URL.

# Previous Versions #
original: http://bloggergreetbox.googlecode.com/files/TextToBeDisplayedDiv-minv3.0.js
mine: http://fav.consumedconsumer.org/scriptache/bi-TextToBeDisplayedDiv-minv3.0.js

I will include major changes in the file description from now on, so to use it, make sure you change the filenames to reflect the newer versions, that's all you need to do (apart from entering your Blogger blog URL)!
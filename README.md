# Hide WixStudio ads for free
## Code for desktop version
We create the desktop version of the wix studio site.
```
</head><body>
  <title>Title of the site</title>
  <link rel="icon" type="image/x-icon" href="/youriconhere.ico">


<body>
  <iframe src="https://yourname.wixstudio.io/yoursitehere" style="position:fixed; top:-29px; left:0px; bottom:0px; right:0px; width:100%; height:105%; border:none; margin:0; padding:0; overflow:hidden; z-index:999999;">
</iframe>  
   
  </body>
    <script type="text/javascript">
<!--
if (screen.width <= 900) {
document.location = "/mobile.html";
}
//-->
</script>
  


</body></html>

```

## Code for Mobile
Now we create the file that the Desktop one is pointing, this time with the name "mobile.html" (you can name it with whatever you want).

```
<html>
  <title>Title of the site</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <body>
  
     <iframe src="https://yournamehere.wixstudio.io/yoursite" style="    position: fixed;    left: 0px;    top: -30px;    width: 100%;    height: 108%;}">
</iframe>
    
  </body>
</html>
```

## Domain and Hosting
### Domain
Now we need where to host our site. We can use [eu.org](https://eu.org) (but the domain registration is really slow) or [us.kg](http://us.kg), wich I would right now reccomend, even for its compatibility with CloudFlare.
### Hosting
We have our domain. For hosting, right now, I've found only a solution, [FreeHostia](https://www.frehostia.com), but it's pretty stable.
We register on their site (they will not ask for your credit card) and then connect our domain via NameServers in the us.kg's reserved area (dns1.freehostia.com and dns2.freehostia.com).
Now, that we have our domain pointing to Freehostia's nameservers, we can create the html pages of our site, copy & pasting the code above (changing the wixstudio url for every page).
#### SSL
With FreeHostia you can receive a Let's Encrypt certificate, that renews automatically after 90 days.






## Creds:
[Bobojeans Repo](https://github.com/bobojean/Hiding-Wix-Ad-for-Free) that I've updated for WixStudio.


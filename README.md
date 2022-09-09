# RasPi_NOAA-webpanel
Personalise the web panel



This is my personalised webpanel from https://github.com/jekhokie/raspberry-noaa-v2<br>

Replace the origional webpanel located /home/pi/raspberry-noaa-v2/webpanel<br>
with this one<br>

Any changes are made at your own discression

To change the home button link go to 
webpanel\App\Views\base.html<br>
edit the the text in bold <br>
class="nav-link" href="<b>insert homepage here</b>"
<p>

To change the time location<br>
  Go to https://time.is/customize <br>
  set your location and style<br>
  edit files webpanel\App\Views\Captures\index.html and webpanel\App\Views\Passes\index.html<br>
  and replace the code<br>
<code>
a href="https://time.is/Clarinbridge" id="time_is_link" rel="nofollow" style="font-size:16px;color:white">Clarinbridge:</a>
span id="Clarinbridge_z70b" style="font-size:16px;color:white"></span>
script src="//widget.time.is/en.js"></script>
script>
time_is_widget.init({Clarinbridge_z70b:{template:"TIME<br>DATE<br>SUN", date_format:"dayname daynum/monthnum/yy", sun_format:"Sunrise: srhour:srminute Sunset: sshour:ssminute<br>Day length: dlhoursh dlminutesm", coords:"53.2286100,-8.8775000"}});
  </script></code><br>
<p>
When you think you are ready open open terminal and type<br>
cd raspberry-noaa-v2/<br>
./install_and_upgrade.sh
<p>
After changes have taken effect, you should now have a Dark themed webpanel.<br>
If you dont like it and want to revert back to the original<br>
You can replace the files with the original at https://github.com/jekhokie/raspberry-noaa-v2/tree/master/webpanel.

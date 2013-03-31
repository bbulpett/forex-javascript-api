forex-javascript-api
====================

This is example of receiving real time Forex data feed from <a href="http://apirates.com/">Apirates.com</a> in javascript using JSONP API.

JSONP API:

For the current bar:

<code><a href="http://api.apirates.com/jsonp/update/myCallback">http://api.apirates.com/jsonp/update/myCallback</a></code>

For history bars:

<code><a href="http://api.apirates.com/jsonp/history/M1/myCallback">http://api.apirates.com/jsonp/history/M1/myCallback</a></code>
<code><a href="http://api.apirates.com/jsonp/history/M5/myCallback">http://api.apirates.com/jsonp/history/M5/myCallback</a></code>
<code><a href="http://api.apirates.com/jsonp/history/M10/myCallback">http://api.apirates.com/jsonp/history/M10/myCallback</a></code>
<code><a href="http://api.apirates.com/jsonp/history/M15/myCallback">http://api.apirates.com/jsonp/history/M15/myCallback</a></code>
<code><a href="http://api.apirates.com/jsonp/history/M30/myCallback">http://api.apirates.com/jsonp/history/M30/myCallback</a></code>
<code><a href="http://api.apirates.com/jsonp/history/M60/myCallback">http://api.apirates.com/jsonp/history/M60/myCallback</a></code>


<strong>How JSONP works?</strong>

Add script with link to JSNOP Apirates API to your page.
The last parameter "myCallback" can be anything else you want.
```
<script type="text/javascript" src="http://api.apirates.com/jsonp/update/myCallback"></script>
```
Then define function "myCallback" or any other function, it depends on what parameter you submited on the end of API call.
```
function myCallback(data){}
```

After the page loads, "myCallback" will be called and parameter "data" will contain Forex data for current bar in this case.

See the index.html example for better understanding and read more about JSONP on <a href="http://en.wikipedia.org/wiki/JSONP">wiki</a>

BlastBestBuy
============

<strong>Overview</strong><br>
This is a game created during a 24 hour hackathon over the weekend of July 19th-20th. I used Unreal Engine 4 and the VaRest plugin for REST API integration. This is more of a proof of concept than anything else. It shows how easily one can implement calls to REST API's and take action based on the response. I have removed my API keys from the application before uploading to GitHub, so there are a couple of steps one would need to take before this code will work.

<strong>Requirements</strong><br>
Unreal Engine 4 Editor access (obviously?)<br>
<a href="https://developer.bestbuy.com/" target="_blank">Best Buy developer portal</a> access to get your own API key<br>
...and that should be about it.

<strong>Setup</strong><br>
Everything is implemented in Blueprint, so there is no code to touch directly. To get this working, the Spawn Volume and Category blueprints will need to be edited. There is a variable named APIKey in each one. The proper entry will read:<br>
&apiKey=[your api key]<br>
without the <>'s. Just so we are clear, if your API key is 1234, you would put &apiKey=1234 in the default text of both variables. This will allow your game to communicate with the Best Buy system and return the results properly.

<strong>Misc</strong><br>
Before you point out the inconsistencies or things that should have been done differently... yes, I know :) There are many ways I could have optimized this, and many things that should have been implemented in a better way. If I would have had more time to work on it, some of those may have been completed. There are many inconsistencies in how things are implemented or called, mostly because I was trying out different methods to achieve the same purpose. As I said, this was a proof of concept and so I was doing a bit of experimenting.<br>
<br>
That said, I want to give much thanks to the awesome <strong>ufna</strong> for creating the plugin that made this possible. The <a href="https://forums.unrealengine.com/showthread.php?13509" target="_blank">VaRest plugin</a> allowed me to call REST API's and decode the JSON response through Blueprint! It was the only way I was able to get this up and working in such a short time.

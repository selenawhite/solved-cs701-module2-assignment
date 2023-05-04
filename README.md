Download Link: https://assignmentchef.com/product/solved-cs701-module2-assignment
<br>
<ul>

 <li>When the term <em>lastName</em> is referenced in an assignment, please replace it with your last name.</li>

</ul>

<strong>You are strongly encouraged to add comments into your program!</strong>

Create a new folder named HW2_<em>lastName. </em>Write the following programs in this folder. <strong>Scenario: </strong>

You decided to release the dove residing in your birdcage. But, you are keen in tracking the flight of the bird. So, you tied a sensor tag to the poor bird and decided to write a HTML5 application to monitor its path. Since you neither have the bird nor the sensor, you decided to simulate the path. <strong> </strong>

<h1>Part 1 – Geolocation (50 Points)</h1>

Using the HTML5 Geolocation API, write the LocationTracker.html and the associated Javascript file LocationTracker.js. You are free to use the html5.css from the samples.

The initial rendering of the HTML page is shown below with placeholders for the location details and the Google map.




<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/411.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/411.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>When the <em>Start</em> button is clicked, get the current position using the Geolocaiton API and display the initial location in the map as shown below. After the initial location is displayed, use the <em>setInterval</em> method to invoke your method <em>updateMyLocation</em> every 5 seconds. The <em>Start</em> button is disabled from now on.

The <em>updateMyLocation</em> method simulates the changes in the latitude and longitude as follows. Generate two random numbers using Math.random() and divide each by 100. These two numbers represent the changes in the latitude and longitude. Modify the current location by adding the latitude value and subtracting the longitude value. This will make the bird only fly in the NorthWest direction. If you are on the Northern border or the Western border, feel free to keep the bird over the United States (or your country) by the appropriate changes to the current location. Update the current location in the HTML and also draw the path in the Google Map as shown in the second figure below.




<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/945.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/945.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>










<strong>           </strong>

<strong>Part2 – HTML5 Drag and Drop and Local Storage (50 points) </strong>

<strong>Democrat and Republican senators voting by their party lines through Drag and Drop. </strong>

The application presents a list of senators and two areas representing Democrats and Republicans. The senators are dragged and dropped into their respective areas.

The initial list is loaded through AJAX from the partyList.xml file (provided in the samples). Each senator is converted to a JSON object keeping track of the properties <em>name</em>, <em> party</em>, and <em>voted</em> (true or false). The list of senators is then stored in local storage. Whenever a senator is dragged and dropped into their respective area, the JSON object is updated as voted and the list of senators is updated in the local storage. When the application is loaded, the local storage is first checked. If the data is there, the list of senators is loaded from the local storage, otherwise the AJAX call is made.

When the data exists in the local storage and the application is loaded, the senators already dragged into their respective areas should also be populated. Make sure you test this case.

Write the partyWise.html and partyWise.js for the application’s functionality.

The structure of partyList.xml is shown below.

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/225.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/225.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>The initial screen when the application is loaded is shown below. AJAX call is made to load the senator list.

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/185.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/185.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>At this point, the local storage should contain the senators entry:

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/354.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/354.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>If the application is refreshed, the data should be loaded from the local storage:

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/887.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/887.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>




After a few drag and drops, the application looks like this:

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/897.png?w=980&amp;ssl=1" class="aligncenter lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="aligncenter" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2019/09/897.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>

Note that the democrats can only be dropped into the Democrats area. Similarly for the Republicans. You cannot drag and drop the member already voted.

If the application is quit and then reloaded, the application should resume from the last snapshot.
# WURFLjs-demo
A quick getting started template for wurfl.js

//It is the same wurfl distributed by ScientiaMobile.
/* WURFL.js is a JavaScript file that provides information about the device that is accesing your page. Whether it is a desktop browser, a tablet, a mobile phone, a smart TV, game console or someone with his wristwatch.
*/

First, include the script in your markup (https is suported):


<script type='text/javascript' src="//wurfl.io/wurfl.js"></script>
...and start JavaScripting:


console.log(WURFL);
You can for example use the object to check if it is a mobile device like this:

if(WURFL.is_mobile){
	//dostuff();
}
View source on this page to see more examples on how to use WURFL.js.

For this particular browser/device, the WURFL object looks like this:

{"is_mobile":false,"complete_device_name":"generic web browser","form_factor":"Desktop"}
Below are the capabilities and values you can make use of.

complete_device_name
The name the device is known by. Typically make and model, a "group" of devices, or a more generic definition.
form_factor
Desktop
App
Tablet
Smartphone
Feature Phone
Smart-TV
Robot
Other non-Mobile
Other Mobile
is_mobile
true or false. True if the device is a tablet, or other mobile device.
Further, you can control caching by adding this parameter to the query string.

debug=true
Any cache is switched off. Useful while developing

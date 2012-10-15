#jquery.bgpos.js

##Purpose
jQuery does not support animating the css property background-position with it's standard animate() method.  This plug-in will allow you to do that.

##How To Use
There is a demo application included in the repo.  To use the demo application, it will have to be served by a web-server and opened in your browser.  I recommend XAMPP in Windows, or a standard LAMP stack with Apache in *nix.
    
	$(function() {
			
		$("#demo").hover(function(){
			$(this).animate({ backgroundPosition : "201 0"});
		}, 
		function(){
			$(this).stop()
			$(this).animate({ backgroundPosition : "0 0"});
		});
		
	});

##Compatibility
Currently tested with:
* jQuery versions:
    * 1.7.2
	* 1.8.2
* Browsers:
	* Firefox 16
	* Chrome 22
	* Internet Explorer 9 (in standards mode)

##Credits
For licensing info, see the included LICENSE.md

The original jquery.bgpos by Alexander Farkas is hosted at http://code.google.com/p/exteenscript/downloads/detail?name=jquery.bgpos.js&can=2

It is not maintained as far as I can tell and is currently incompatible with jQuery 1.8.x.  You can read my original blog post here: http://nelsonwells.net/2012/08/using-bgpos-js-with-jquery-18
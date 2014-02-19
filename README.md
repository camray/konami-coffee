Konami-JS
=========
# This is a fork of [konami-js](https://github.com/snaptortoise/konami-js) into coffeescript.

You can set either the URL to redirect to OR the function to execute when you instantiate the class:

	var easter_egg = new Konami('http://your-special-easter-egg-website.com');
	
OR:

	var easter_egg = new Konami(function() { alert('Konami code!')});

A passed string is assumed to be the URL to redirect to. A passed function will be executed when the code is successfully entered:

#### Overview

Every site should have an implementation of the Konami Code. It makes things more fun. If you're unfamiliar with it, the Konami Code is a "cheat code" that appeared in many of Konami's video games going all the way back to 1986.  It was typically entered on a Nintendo controller. Recently, ESPN received attention for the funny, flashy things that would happen when the code was entered on their website. Those shenanigans were the inspiration for whipping up this script.

#### Gesture Support

As of version 1.1, Konami-JS includes support for gestures on iOS and Android devices.  Technically the code becomes "up, up, down, down, left, right, left, right, tap, tap, tap," on these devices but that's close enough!

Support for touch gestures is automatically loaded when `konami.load()` is called.  See the [example page](http://snaptortoise.com/konami-js) for details on how to deliver touch-specific easter eggs.
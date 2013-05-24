# _litestrap
### Bare-Bones CSS styling and utilities to get a site off the ground.

I got tired of re-writing the same utilities in every css file I touch, so I put this together.  It's a collection of easy-to-remember, easy-to-use classes that can help you get started on your next project.

## What this isn't

This isn't meant to be a 'do everything for me' CSS library.  This is only for basic utilities that won't get in your way when you're putting together something new.  I may extend this a bit in the future, but the idea for now is to keep it as simple as possible.  If you want something that will do more, please by all means use [inuit.css](http://inuitcss.com/) or [Bootstrap](http://twitter.github.com/bootstrap/) instead - a lot of work was put into those, and far more by comparison than my humble contribution can boast.  I admire these libraries but choose not to use them sometimes - which is why I made litestrap. :)

litestrap doesn't even include a real grid - just a collection of sizes. It's easy to put one together with litestrap and SASS/LESS/stylus though.  If you're using a preprocessor, just copy the class list and nest it in your grid wrapper class (OH THE HORROR).  

```
/* Sometimes I like to use .gw like inuit.css does */
.grid-wrapper, .gw {
	@extend .clearfix; 
	clear: both; 
	margin-left: -20px; 	
	/* litestrap size classes */
	.whole, .half, .third, .twothird, .twothirds, .quarter, .threequarter, .threequarters, .sixth, .eighth, .ninety, .eighty, .seventy, .sixty, .fifty, .forty, .thirty, .twenty, .ten {
		padding-left: 20px;
	}
```

The sizes all use border-box styling anyway so this shouldn't break anything that isn't IE7.  You could also depend on a different class for your grid, so it would look very familiar to inuit.css users ...

```
.gw {
	@extend .clearfix; 
	clear: both; 
	margin-left: -20px;
	.g {
		padding-left: 20px;
	}
}
```

## Installation

Well I guess you could just grab the raw version of litestrap.css here on github.  Either include it with your preprocessor or lump it in with the rest of your css and make a big fun mess! :)

I've also included a reset.css because litestrap doesn't do any of that either and if you're starting with litestrap you'll probably need it!  I don't take any credit for the reset - I honestly don't remember where it came from and I'll be happy to update this readme when I figure it out.
# _litestrap
### Helper classes that are actually helpful.  An extra-responsive framework that makes sense (I think).

I got tired of re-writing the same utilities in every css file I touch, so I put this together.  It's a collection of easy-to-remember, easy-to-use classes that can help you get started on your next project.  The idea is to be a helpful starting point, and ideally something that you can just use instead of having to go back and see how things are spelled all the time.  (e.g. a two thirds grid can be declared with .twothird or .twothirds, because honestly who hasn't forgotten an 's' here and there)

## What it does

litestrap provides common grid widths with simple names.  It uses ems everywhere instead of pixel-sizing, because ems are cooler.  (They also respond a lot better to user customization).  _litestrap also auto-collapses all grid widths for mobile, and gives you some options to change grids for different device widths.  This is not always desireable for every project, but for many simple projects this is the desireable behaviour.  If you don't want that, just snip out the media queries for your own use. :)

## What this isn't

This isn't meant to be a 'do everything for me' CSS library.  This is for basic utilities that won't get in your way when you're putting together something new.  I've begin extending this as good ideas come to me, but it's far from complete.  If you want something that will do more, please by all means use [inuit.css](http://inuitcss.com/) or [Bootstrap](http://twitter.github.com/bootstrap/) instead - a lot of work was put into those, and far more by comparison than my humble contribution can boast.  I admire these libraries but choose not to use them sometimes - which is why I made litestrap. :)


## Installation

Well I guess you could just grab the raw version of litestrap.css here on github (as well as any of the other optional css extenders in css/_ls).  Either include it with your preprocessor or lump it in with the rest of your css and make a big fun mess! :)

I've also included a reset.css because litestrap doesn't do any of that either and if you're starting with litestrap you'll probably need it!  I don't take any credit for the reset - I honestly don't remember where it came from and I'll be happy to update this readme when I figure it out.
> @grahamzibar presents:
>
>	```
>	 _______  _______  _______  _______           _______           _______
>	(       )(  ___  )(  ____ )(  ____ )|\     /|(  ____ \|\     /|(  ____ \
>	| () () || (   ) || (    )|| (    )|| )   ( || (    \/| )   ( || (    \/
>	| || || || |   | || (____)|| (____)|| (___) || (__    | |   | || (_____
>	| |(_)| || |   | ||     __)|  _____)|  ___  ||  __)   | |   | |(_____  )
>	| |   | || |   | || (\ (   | (      | (   ) || (      | |   | |      ) |
>	| )   ( || (___) || ) \ \__| )      | )   ( || (____/\| (___) |/\____) |
>	|/     \|(_______)|/   \__/|/       |/     \|(_______/(_______)\_______)
>
>	```

* version 0.1.0 - ALPHA
* https://www.github.com/grahamzibar/Morpheus


* ![What if I told you this is not an animation library](https://www.github.com/grahamzibar/Morpheus/morpheus.jpg "Move your mouse elsewhere.")

## Animation libraries are cool!  But this isn't really that.

This is more of a utility.  This appends methods to the `HTMLElement` class in
order to provide a more semantic means (on the JavaScript side of things) to
generate transitions/transforms/animations.  This way, we're not constantly
switching back and forth between CSS, JavaScript, and HTML.  We simply add
the transitions we need, and then set our styles accordingly.

**Morpheus** optimizes this by completely decoupling the storing of the desired
view (transforms, transitions, styles, etc.) away from the _renderer_. The
`morpheus.Renderer` class is meant to be overridden according to the platform
you are targeting.  By default, `morpheus.Renderer` accounts for WebKit, but
this will moved to a separate file called `CSS3Renderer.js` very soon.

## TODO: finish this documentation
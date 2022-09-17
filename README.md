
# A Timber Starter Theme

An opnionated and dirty WordPress Starter theme based on Timber allowing Twig templating for WordPress.

This is a bit rough and needs some clean up. The usual caveats apply. Use at your own risk.


## Installing the Theme

Install this theme as you would any other, and be sure the Timber plugin is activated. 

### Two Methods for installing the Timber plugin

#### 1. Install the plugin
1. Make sure you have installed the plugin for the [Timber Library](https://wordpress.org/plugins/timber-library/) (and Advanced Custom Fields - they [play quite nicely](https://timber.github.io/docs/guides/acf-cookbook/#nav) together). 
2. Download the zip for this theme (or clone it) and move it to `wp-content/themes` in your WordPress installation. 
3. Rename the folder to something that makes sense for your website (generally no spaces and all lowercase). You could keep the name `timber-starter-theme` but the point of a starter theme is to make it your own!
4. Activate the theme in Appearance >  Themes.
5. Do your thing! And read [the docs](https://timber.github.io/docs/).

### 2. Use Composer

`composer require timber/timber`

The installer uses an old version of PHP. If you run into problems, try the --ignore-platform-reqs flag.

`composer require timber/timber --ignore-platform-reqs`

## What's here?
`src/` source files for SASS, JS and images

`static/` is where you can keep your unprocessed static front-end scripts.

`templates/` contains all of your Twig templates. These pretty much correspond 1 to 1 with the PHP files that respond to the WordPress template hierarchy. At the end of each PHP template, you'll notice a `Timber::render()` function whose first parameter is the Twig file where that data (or `$context`) will be used. Just an FYI.

`bin/` and `tests/` ... basically don't worry about (or remove) these unless you know what they are and want to.

## Adding Node dependencies

You will need to install Node dependencies to run the Gulp commands.

`npm install` or `yarn install`

## Customising the theme

Edit the comments at the top of `src/sass/style.scss` to reflect your theme.

* https://developer.wordpress.org/themes/basics/main-stylesheet-style-css/

## Other Resources

* [The Timber starter this theme is based on](https://github.com/laras126/timber-starter-theme/tree/tackle-box) of the starter theme has some more example code with ACF and a slightly different set up.
* [Twig for Timber Cheatsheet](http://notlaura.com/the-twig-for-timber-cheatsheet/)
* [Timber and Twig Reignited My Love for WordPress](https://css-tricks.com/timber-and-twig-reignited-my-love-for-wordpress/) on CSS-Tricks
* [A real live Timber theme](https://github.com/laras126/yuling-theme).
* [Timber Video Tutorials](http://timber.github.io/timber/#video-tutorials) and [an incomplete set of screencasts](https://www.youtube.com/playlist?list=PLuIlodXmVQ6pkqWyR6mtQ5gQZ6BrnuFx-) for building a Timber theme from scratch.

## Thanks

* [Barebones CSS](https://acahir.github.io/Barebones/): A revamped version of GetSkeleton

* [Kitty Giraudel's 7-1 SASS Boilerplate](https://github.com/KittyGiraudel/sass-boilerplate)
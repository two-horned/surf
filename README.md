# My build of suckless's dmenu

This build includes some patches (Mentioned below)

## surf - simple webkit-based browser

surf is a simple Web browser based on WebKit/GTK+.

### Requirements

In order to build surf you need GTK+ and Webkit/GTK+ header files.

In order to use the functionality of the url-bar, also install dmenu[0].

### Installation

Edit config.mk to match your local setup (surf is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install surf (if
necessary as root):

    make clean install

### Running surf

run
	surf [URI]

See the manpage for further options.

### Running surf in tabbed

For running surf in tabbed[1] there is a script included in the distribution,
which is run like this:

	surf-open.sh [URI]

Further invocations of the script will run surf with the specified URI in this
instance of tabbed.

[0] http://tools.suckless.org/dmenu
[1] http://tools.suckless.org/tabbed

## Patches credits
- [playexternal](https://surf.suckless.org/patches/playexternal/)
  - Daniel Nakhimovich - dnahimov@gmail.com
- [bookmarks](https://surf.suckless.org/patches/bookmarking/)
  - Julien Steinhauser - julien.steinhauser@orange.fr
  - blut
  - Alexis Ben Miloud--Josselin; panpo; alexisbmj+code at protonmail dot com.
- [spacesearch](https://surf.suckless.org/patches/spacesearch/)
  - Dmitrij D. Czarkoff czarkoff@gmail.com
  - Alexis Ben Miloud--Josselin; panpo; alexisbmj+code at protonmail dot com.

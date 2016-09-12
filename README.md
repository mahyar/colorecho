# colorecho: Wrap your strings in terminal color codes.

The same code should work in python2.7 & python3.x.

```
$ colorecho -h
usage: colorecho [-h] [-r] [-b BACKGROUND_COLOR] [-m MODIFIER]
                 colorName [string [string ...]]

Prints terminal colorized versions of your strings.  For example:

$ colorecho red "Hello fine sir"
Hello fine sir
$ colorecho -b 180 -m blink 1 "Hello fine sir"
Hello fine sir
$ colorecho --raw -b 180 -m blink red Hello fine sir
'\x1b[31;48;5;180;5mHello fine sir\x1b[0m' 
$ cowsay Hello fine sir | colorecho -m blink green 
<A blinking green cow who says: "Hello fine sir">

positional arguments:
  colorName             The name of the color you want. You can put a number
                        between 0..256 if your terminal supports it or choose
                        from these names: blue, light-green, default, light-
                        yellow, light-gray, light-red, yellow, light-blue,
                        dark-gray, light-cyan, black, cyan, green, magenta,
                        light-magenta, white, red
  string                Whatever text you want to colorize.

optional arguments:
  -h, --help            show this help message and exit
  -r, --raw             Print raw version of the color string.
  -b BACKGROUND_COLOR, --background_color BACKGROUND_COLOR
                        Set a background color for your text. You can put a
                        number between 0..256 if your terminal supports it or
                        choose from these names: blue, light-green, default,
                        light-yellow, light-gray, light-red, yellow, light-
                        blue, dark-gray, light-cyan, black, cyan, green,
                        magenta, light-magenta, white, red
  -m MODIFIER, --modifier MODIFIER
                        Set a modifier for your text. Choose from these names:
                        dim, underlined, strikeout, bold, italic, invert,
                        hidden, blink. Italic and strikeout is not widely
                        supported in terminals.
```

## Installation

`$ pip install colorecho`

## Other fun terminal toys
* [`lolcat`: Rainbow color your console text!](https://github.com/busyloop/lolcat) `gem install lolcat`
* [`figlet`: Make ASCII console banners.](http://www.figlet.org/) `brew install figlet`
* [`toilet`: A better version of figlet](http://caca.zoy.org/wiki/toilet) `brew install toilet`
* [`cowsay`: Make an ascii cow say your text.](http://www.cowsays.com/)
* [`fortune`: Classic quote printer.](https://en.wikipedia.org/wiki/Fortune_(Unix)) `brew install fortune`
* [`banner`: Make a big dot matrix printer banner text file.](https://en.wikipedia.org/wiki/Banner_(Unix))

# Hue
Hue will help you to print awesomely in terminals.
Hue
Hue Logo

Hue provides a minimal and powerful interface to print colored text and labels in the terminal.
It works with Python 2 as well as Python 3.

What makes hue better than other coloring libraries? Here's a comparison.

Supported Stuff
Following styles are supported

Hue Styles

Following colors are supported

Hue Colors

Following labels are supported

Hue Labels

Installation
You can install hue with pip as follows:

pip install huepy
or with easy_install:

easy_install huepy
Usage
First of all, import everything that Hue has to offer as follows:

from huepy import *
Printing colored text is as simple as doing

print red('This string is red')
Easy right? But what if you want to print italic text? You can simply do this

print italic('This string is in italic')
You can also combine styles and colors

print bold(red('This string is bold and red'))
Output: Output Examples

And what is the use of those labels?
I have been using these labels in projects as a minimal output schema.
If some error occured in your program or something else bad happened you don't need to print the whole line in red. With hue, you can simply do this

print bad('An error occured.')
Take a look at the output of all the labels Label Examples

List of all colors
white, grey, black, green, lightgreen, cyan, lightcyan, red, lightred,
blue, lightblue, purple, light purple, orange, yellow
List of all styles
bold, bg, under, strike, italic
List of all labels
info, que, run, bad, good
Note: Windows versions below windows 10 do not support ANSI escape sequences so the colors will not be printed in command prompt.

Why hue
Because its awesome! Lets print a red colored string in popular coloring libraries:

Colorama
from colorama import Fore
print Fore.RED + 'This string is red'
Termcolor
import sys
from termcolor import colored, cprint
print colored('This string is red', 'red')
Hue
from hue import *
print red('This string is red')
Here's comparison table:

Hue	Colorama	Termcolor
Compatibility	Unix & Windows 10	Unix & Windows	Unix
Ease of use	10/10	4/10	5/10
Bright Colors	Yes	No	No
Note: Colorama and Termcolor print bold styled strings when asked for bright colored strings. On the other hand, Hue supports both bright and bold strings. Also the Ease to use ratings are a result of my own experience and may differ for others.

Contribution
The only thing I think Hue needs is better windows compatibility. So if you can start a pull request for windows support that would be great. Additional colors and labels will be appreciated too.

InPy
Version 1.9
May 27, 2010
Copyright 2008 - 2010 by Jamal Mazrui
GNU Lesser General Public License (LGPL)

Contents

Introduction
Python Modules
Web Client Utilities
Change Log
----------

Introduction

InPy (short for Interactive Python) is a free, console mode environment for testing and evaluating code in the Python language.  InPy seeks to enhance the default shell environment of Python for Windows in ways that make it more productive, especially for screen reader users.  The program works well with a screen reader, since new output to the console is automatically read.  InPy may also be used as a speech-friendly calculator or workspace, since various math and science modules are available for Python, e.g., from the SciPy page at
http://scipy.org

Python is being used as the development language in several accessibility-related projects, including the following:

accessible_output - Library to provide speech and braille output to a variety of different screen readers and other accessibility solutions
http://pypi.python.org/pypi/accessible_output/0.4.1

dragonfly - Speech recognition extension library
http://pypi.python.org/pypi/dragonfly/0.6.5

InPy - A custom Python interpreter optimized for web client utilities
http://EmpowermentZone.com/InPy.zip

latex-access - Making LaTex math syntax more readable with speech or braille
http://latex-access.sourceforge.net

macspeechX - A module to access speech synthesis module on MacOSX
http://pypi.python.org/pypi/macspeechX/1.0

McTwit - A Twitter client for Windows
http://EmpowermentZone.com/mtsetup.exe

NonVisual Desktop Access (NVDA) - A screen reader for Windows
http://www.nvda-project.org/

Orca - A screen reader for Linux and Solaris
http://live.gnome.org/Orca

PyFest - A simple interface to the Festival speech server
http://pypi.python.org/pypi/PyFest/0.1

pytext - Simple text to speech pre-processor
http://dexrow.blogspot.com/2009/06/python-voice-preprocessor.html

pyTTS - Python Text-to-Speech for Windows
http://pypi.python.org/pypi/pyTTS/3.0

pyttsx - Cross platform text-to-speech
http://pypi.python.org/pypi/pyttsx/1.0

Qwitter - a Twitter client for Windows
http://www.qwitter-client.net/

SayTools - Collection of command-line utilities and a COM server to add direct speech messages to Windows applications
http://EmpowermentZone.com/saysetup.exe

speech - A clean interface to Windows speech recognition and text-to-speech capabilities
http://pypi.python.org/pypi/speech/0.5.2

Yet Another Braille Translator
http://pypi.python.org/pypi/YABT/1.0.1

Interested programmers can leverage such existing solutions to increase the availability of software applications that are accessible.

The main code for this project, InPy.py, should work on Python 2.4, 2.5, or 2.6.  Development and testing are currently done with 2.5, so that is the recommended version.

To manually install the program, download the archive at
http://EmpowermentZone.com/InPy.zip
and unzip it into a directory that is convenient to access at a Windows command prompt, e.g.,
C:\InPy

To run the program, execute the batch file InPy.bat.  If you are in its directory, you can just enter
inpy
at the command prompt (capitalization does not matter).  The batch file uses Python 2.5 if it has been installed in the default directory
C:\Python25

Alternatively, you can invoke the program with the latest version of the EdSharp text and code editor, available at
http://EmpowermentZone.com/edsetup.exe

EdSharp includes features for managing indentation in Python.  After picking the Python language with Control+Shift+F5, InPy is available with the Go to Environment command, Control+Shift+G (assuming Python is installed).  If you update an EdSharp installation, press Alt+Shift+0 for new default settings that include InPy support.

InPy is developed with the InteractiveConsole class of the Python language, implementing an interpreter that works like the standard one with additional enhancements.  This includes being able to clear the screen with the cls command.  You can also save output from a session with the log command.

InPy does not import all of the Python standard library.  The following 40 standard and third party modules are imported:

code
comtypes
comtypes.client
configobj
datetime
deliciousapi
feedfinder
feedparser
glob
googlemaps
html2text
htmllib
locale
os
platform
pprint
pywapi
re
simplejson
StringIO
sunlightapi
SunlightApiError
sys
textwrap
time
twill
uri
urllib
urllib2
urlunshort
win32api
win32clipboard
win32com.client
win32com.client.dynamic
win32con
win32console
win32gui
winsound
xml.etree.ElementTree
yahoo.search.term

For anyone interested in learning to program in Python, some useful links are as follows.  The direct download address of the Python 2.5 installer is
http://python.org/ftp/python/2.5.2/python-2.5.2.msi

The main list of Python add-in packages is at
http://pypi.python.org/pypi?%3Aaction=index

A convenient utility called easy_install for adding or updating packages is at
http://pypi.python.org/pypi/setuptools/

A collection of text tutorials on Python is at
http://EmpowermentZone.com/pyth_doc.zip

I invite Python programmers to contribute ideas and code to this open source project.  Below is the online help of this release:

InPy 1.1 by Jamal Mazrui

Type a Python statement or expression, followed by Enter.
A trailing semicolon (;) may be used to seperate multiple statements 
on the same line, though indentation would still 
need to be embedded for a nested block.
The prompt changes from a greater than symbbol (>) to a period (.) 
if more input is needed to complete a statement.

If the output of a command is more than 23 lines of text, 
the display is paused so that it does not scroll off the screen.  
The More? prompt then requests a choice, 
to be followed by Enter.  
Enter the letter y or nothing to answer Yes for the next screen.  
Enter n for No, thereby returning to the > input prompt.  
Enter a for All text, which continues without pausing.  
This is useful when logging the output to a file.

Besides regular Python syntax, this interpreter adds some commands.
A command name is lower case, with a space before any argument, 
which is not quoted.

exit or quit - end this program

cls - clear the screen

exec FileName - execute a Python script file

log FileName - log output to a new file

log off - stop logging

help - display this documentation

Other help features of the standard Python interpreter are available, 
e.g., the help() and dir() functions, 
used either with or without parameters.
----------

Python Modules

The following 111 standard and third-party modules are built into Inpy:

pywinauto
atexit
base64
calendar
caseless
cgi
chrono
cmd
code
codecs
commands
comtypes
comtypes.client
configobj
ConfigParser
copy
csv
ctypes
datetime
dateutil.parser
dateutil.relativedelta
dateutils
deliciousapi
win32api
doctest
feedfinder
feedparser
fnmatch
ftplib
getopt
getpass
glob
googlemaps
html2text
htmlentitydefs
htmllib
httplib
Image
ImageGrab
TiffImagePlugin
locale
logging
lxml
math
mimepost
mimetools
mimetypes
msvcrt
odict
optparse
os
os.path
pathutils
parsedatetime
pickle
pkgutil
platform
poster.encode
poster.streaminghttp
pprint
pythoncom
pywapi
random
re
ConfigParser
readline
robotparser
scrapy
sets
sgmllib
shelve
shutil
signal
simplejson
Skype4Py
sqlite3
standout
string
StringIO
subprocess
sunlightapi
sys
tarfile
tempfile
textwrap
thread
threading
time
tinyurl
twill
types
unicodedata
uri
urllib
urllib2
urlparse
urlunshort
validate
webbrowser
win32api
win32clipboard
win32com.client
win32com.client.dynamic
win32con
win32console
win32gui
winsound
xml.dom
xml.etree
yahoo.search.term
zipfile

----------

Web Client Utilities

Many .py files are included in the distribution as useful examples of what InPY can do with a relatively small script file.  They are used, for example, in the Web Client script package for Window-Eyes
https://www.gwmicro.com/Script_Central/Scripts/Script_Details/?scriptid=1278

and in the Firefox Max scripts for JAWS
http://EmpowermentZone.com/FxMax.exe

to implement a Web Client Utilities command.  The JAWS command, Control+JAWSKey+Space, is similar to the JAWS ResearchIt command, JAWSKey+Space.  The web client utilities are handy ways of getting useful information from free web 2.0 services.  The following 35 utilities are installed (for efficient navigation, each has a unique initial character, which may be a letter, digit, or symbol):

!Odd News - Get recent news items that are strange but true via reuters.com.

@DomainLookup - Get authoritative information about the registrant of an Internet domain name, e.g., AccessibleWorld.org.  Note that some firewalls block this utility because it uses a different port than standard HTTP requests.  This uses the free WhoisThisDomain utility from
http://nirsoft.net/utils/

#SportScores - Pick a sport from a list and go to the corresponding page on ESPN.com with recent news and scores.

$Product Search - Enter keywords that describe a product and go to its matching web page on amazon.com.

-TimeInternational - Enter a location (e.g., specified as city, country) and get the current time there via google.com.

=UnitConversion - enter a source value, e.g., 10 miles, and a target unit, e.g., kilometer, and get the converted result via google.com.  This works for currency units as well as physical measurements.

1 Mile Stories - Get recent blog or news stories about a location and surrounding area within a one mile radius via the outside.in web service.  Enter a location such as your home address on one line by using a comma and space between segments that you might otherwise type on separate lines.

508 Check - Check a web page for compliance with accessibility standards of the United States Government (Section 508 of the Rehabilitation Act), as well as standards of the World Wide Web Consortium (W3C).  This checks a web page against 508 standards via CynthiaSays.com (the site limits checks to one per minute from the same client).  It also includes the report of Wave, a web evaluation checker from WebAim.org.

0Captcha - Submit a captcha to solona.net ( a free account is required), and have the text solution copied to the clipboard so you can paste it into a web form.  The utility waits up to 90 seconds for a human operator to respond.  This utility is typically executed from within a browser that is displaying a captcha, though any .png file on disk may be submitted.

Address Lookup - Search for addresses of organizations meeting geographic and other criteria via jigsaw.com.  This prompts for an organization name, area code, zip code, web site type, and fortune rank.  Fill in one or more fields for the search.  For example, input gov for the web site type in order to get government organizations, or 500 in the fortune field to get companies in the top fortune 500.

Business Reviews - Search for reviews of a business specified by a phone number via yelp.com.

Common URLs - Show a list of the 100 most commonly referenced URLs on Twitter at present via TweetMeme.com.  These typically point to news stories that people have been retweeting.

Driving Directions - Input a starting and ending location, and get a list of steps to get there by car (a blind person might share this with a friend or cab driver).  The location may be specified as a street address in any country.  The utility prompts for a starting and ending address, uses the Google Maps API, and puts the estimated distance, duration, and steps in the viewing area.  Specify an address as if you were addressing an envelope except for a comma rather than return between each line, e.g.,
1400 East-West Highway, Silver Spring MD 20910, USA

USA is assumed as the country if not specified.

EnglishDictionary Lookup - Get definitions and other information about a word via wiktionary.com.

Feed Find - Get a list of RSS and ATOM feeds made available by a web site.  This prompts for a web source and returns a list of RSS or ATOM feeds found.  An http:// prefix is assumed if not specified.  For example, entering
cnn.com

finds two RSS feeds related to top stories and latest stories.  You can open a feed url to read recent content, or subscribe with a feed reader for regular updates.

Google Search and Set Suggestions - Propose a Google search and get a list of popular searches that are similar.  Also Get a list of terms that may be part of the same set.  For example, enter a comma-separated list of U.S. presidents and let Google suggest a more complete list.

Horoscope Reading - Input a zodiac sign (e.g., Sagittarius) and get a horoscope for today via my.horoscope.com.

Interesting Places - Get a list of nearby places to eat, shop, or visit via NextStop.com.  This prompts for a location, which can be in the city, state format, or a complete address with commas seperating postal address lines.  Also input the distance in kilometers to search from that location, and any words that you want to narrow the search, e.g., Chinese for that type of food.  An excerpt from a review of each place is also included, if available.

Journalist World Reports - Get world headlines from multiple web sources:  the BBC, CNN, Christian Science Monitor, New York Times, Reuters, and Yahoo.  A structured text file is generated containing a section of news items from each source.  Each item has a title, summary, and URL for the full article.

KnowledgeWikipedia - Input a topic and get a Wikipedia article as both a web page and a text file.

Language Translation - Translate text you specify, between about 100 different languages.  You can quickly understand what a foreign phrase means or how to write it.  This uses the Google Translate API to translate text among about 100 natural languages.  By default, the choice for the source language is unknown and automatically inferred by Google.  You pick the target language, and either enter or paste text in the multi-line edit box.

Members of Congress - Based on a U.S. zip code, get a list of House and Senate members with various data including committee assignments and contact information via SunlightLabs.com.

Neighborhood Search - Search for places near a location, e.g., restaurants with a particular cuisine near an address you are visiting (anywhere in the world).  This prompts for an address in the same format as Driving Directions and also for one or more keywords specified as if searching on Google, e.g.,
seafood steak

to find restaurants in the area that serve both seafood and steak.

Original URL - Get the original version of a URL, e.g., one that was shortened for sharing in a tweet.  This does the reverse of the Short URL utility, prompting for a URL, converting it, and copying the result to the clipboard.

Physician Online - Enter a medical topic and go to a matching web page on WebMD.com.

Quotes of the Day - Get daily food for thought from famous quotes and their authors.  This Shows a humorous quote from IHeartQuotes.com, as well as several motivational quotes from QuotationsPage.com.

Recommended URLs - Based on a topic word, get a list of currently popular URLs that people are saving as bookmarks via delicious.com.

Short URL - Get a shortened version of a URL via j.mp.com, e.g., so you can share it in a tweet and have more text to type within the 140 character limit.

Trend Topics - Get a list of currently popular topics on Twitter via LetsBeTrends.com.

Url Downloads - Batch download multiple urls based on an initial page address and the extensions of files linked to it.  This puts a space-separated list of extensions found in an input box.  Edit it so that only the extensions you want remain.  The utility then puts a list of those links in a multiple-selection listbox, showing the link text and URL for each.  The items are all selected by default, but you can use arrow keys and Spacebar to unselect ones as desired.  The next dialog prompts for a folder for saving the files, which will be remembered as the default choice the next time.  The utility says the name of each file as it is being downloaded.

Virtual White Pages - Search the white pages of U.S. phone books for listings of residential phone numbers and postal addresses via WhitePages.com.

Weather Check - Get a summary of current and forecasted conditions for any location via wunderground.com.  This works with city, country locations as well as U.S. zip codes.  

Xtra Word Info - Get definitions, usage examples, and origins of a word.  This shows definition and examples via Wordnik.com; synonyms and antonyms via words.BigHugeLabs.com; and etymology via etymonline.com.

Yahoo! Term Extractions - Get noteworthy noun phrases contained in a web page via yahoo.com.

Zoom Info - Search for employment contacts by name or email address via ZoomInfo.com.

Each web client utility is defined in a script file written in the Python language.  The file name begins with the WebClient_ prefix and ends with the .py extension, e.g.,
WebClient_508Check.py

The Python script file is run with a custom Python interpreter, InPy.exe, which is also available separately at
http://EmpowermentZone.com/InPy.zip

That package also includes a Console mode version, InPyC.exe, to aid development of Python scripts.  If run without parameters, it opens an interactive shell for testing commands and running scripts, similar to the full python.exe interpreter.  The source code file, InPy.py, imports various web2.0 libraries, and defines many convenience functions.

Web client utilities may be added to the list of available ones by using the same naming convention, e.g.,
WebClient_MyNewScript.py

The Web Client Utilities command remembers the last utility you chose, making it the default in the list.  The information obtained by the utility is automatically saved in a text file and opened in your text editor (the program associated with .txt files in the Windows registry).  Some utilities also open a web page automatically in your default browser.

Note that, at this point, there is not much error checking in the web client utilities, so if a web service returns no useful information for a particular query, a utility may show an error message rather than indicating that no information was available.  If you consistently get errors regardless of the search parameters, please email the error log file, InPy.exe.log.  Errors get appended to this file, so if you want to isolate the error message for a particular utility, delete the log file before running it.
----------

Change Log

Version 1.9 on May 27, 2010
Fixed WebClient_=UnitConversion.py

Version 1.8 on April 14, 2010
Fixed or enhanced the following web client utilities:  Neighborhood Search, OriginalUrl, and ZoomInfoContactSearch.  Increased the documentation on all such utilities.

Version 1.7 on March 17, 2010
added several Python-based, accessibility-related projects to the list in the Introduction section of this documentation.  Added scrapy module for screen scraping from
http://scrapy.org

Added a section of documentation that lists all standard and third- party modules built into InPy.

Version 1.6 on March 10, 2010
Added several Python Modules -- the complete list is the set of import statements at the start of Inpy.py.  Version 1.5 on February 11, 2010
Fixed the following functions:  StringConvertToUnixLineBreak, StringConvertToWinLineBreak, UrlGetBaseDomain.  Added the following functions:  GoogleAddressToLatLng, GetRssItems.  Added the following utilities:  1MileStories, !OddNewws, PhysicianOnline, ProductSearch, and JournalistWorldReports.

Version 1.4 on February 9, 2010
Added WebClient_LanguageTranslation.py and WebClient_UrlDownloads.py.  Made corrections to the following functions:  IniFormDialogMemo, IniFormGetSection, PyString, VtCreateList, WebRequestGetToString, and WebUrlToFile.  Fixed initial index selection in IniForm.exe dialogs.

Version 1.3 on February 6, 2010
Added WebClient_KnowledgeWikipedia.py and WebClient_HoroscopeReading.py.  Fixed HtmlGetText and RegExpExtract functions.  Added web address for Qwitter and McTwit to the list of Python projects in this documentation.  Added setup.py and RunSetup.bat, which are used in building InPy.exe and InPyC.exe.

Version 1.2 on February 4, 2010
Removed debugging code affecting the utilities WebClient_EnglishDictionaryLookup.py and WebClient_MembersOfCongress.py.

Version 1.1 on February 3, 2010

The InPy.py source code now imports various Python libraries for accessing free web 2.0 services, and defines many convenience functions.  Renamed the console mode executable to InPyC.exe and Included a GUI mode version named InPy.exe.  20 WebClient_*.py files are also included.  The command line syntax is

InPy CodeFile InputFile OutputFile

If not specified, InputFile has the same name as CodeFile except for a .ini (rather than .py) extension.  Similarly, OutputFile would have a .txt extension.  Code inside CodeFile can refer to the variables sCodeFile, sInputFile, and sOutputFile.  See the examples, and consider using one as a starting point for a new script.

Added IniForm.exe, SayLine.exe, and SayFile.exe as support utilities.  Canned dialogs using IniForm include ones for multiple input boxes, single or multiple selection listboxes, opening or saving files, and browsing for a folder.  Look for functions with the IniFormDialog prefix in InPy.py.  IniForm documentation is included in the file IniForm.txt.

SayLine and SayFile support direct speech messages using the API of an active screen reader such as JAWS, System Access, or Window-Eyes.  SayLine takes the string to speak as a command line parameter, whereas SayFile speaks the content of the file name passed on the command line.  More information about these utilities is in the SayTools package, available at
http://EmpowermentZone.com/saysetup.exe

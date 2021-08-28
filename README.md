# password-generator
Generate unique and complex passwords

A password generator creates unique and complex passwords.  Today while many password managers have this built in, I wanted a tool with some unique requirements and hence this was born 

1.  Support for CLI on my \*NIX platforms
2.  Support for unique types of passwords such as type with left hand only or type with right hand only
3.  Support for exposing it as a QRCode so it can be transferred to my mobile phone from my screen.
4.  Ensure that the generated password is reasonably secure by checking it againt Tory Hunt's [Have I been Pwned](https://haveibeenpwned.com/About) site

I had written this for my personal use but decided to open source it in a
fairly open MIT license so you can take and modify it for your own use as well.

# Similar Tools
On linux there are a bunch of tools.  pwdgen, xkcdpass, diceware.  The funny
and innovative one is the xkcdpass which came out of the [XKCD.936 comic](https://xkcd.com/936/).  

# Developer Notes

1.  Requires Python 3.7 or greater
2.  Uses two libaries, pyqrcode - for qrcode generation and pyperclip - for clipboard.
3.  I use [Poetry](https://python-poetry.org/) for dependency management.  You
    should too!
4.  I have also added a requirements.txt for people who use a simple
    requirements file.  You can generate it from Poetry with
    ```poetry export -f requirements.txt > requirements.txt```


# winid
A Python script to query for Windows Event IDs and their description.

# Usage

```
usage: winid.py [-h] id

A simple Python script to determine the meaning of Windows event IDs.

positional arguments:
  id          Usage: winid.py 6416,6417,6418 Use this command to enter however
              many IDs you want separated by commas and get back a description
              of what those IDs mean along with a reference for more
              information.

optional arguments:
  -h, --help  show this help message and exit
```

# Example Output
```
exampleuser@examplegroup ~ % python3 winid.py 4768,4771,4625           
==================================================

4768 - A Kerberos authentication ticket (TGT) was requested
Reference: https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=4768

==================================================

4771 - Kerberos pre-authentication failed
Reference: https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=4771

==================================================

4625 - An account failed to log on
Reference: https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=4625

==================================================
```

# Tips for MacOS

- Command double click any links within the terminal to navigate to the URL via web browser.
- Create an alias via .zshrc in to make it easier to run the tool from any directory!

Example .zshrc file:
```
alias winid="python3 ~/tools/winid.py"
```

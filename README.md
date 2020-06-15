# Xkeys (BurpSuite Extension)
<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/result.png">

## Description
A Burp Suite Extension to extract interesting strings (key, secret, token, or etc.) from a webpage. and lists them as information issues.

Type : passive scanner

# Setup
<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/install.png">

- Setup the python environment by providing the <a href="https://www.jython.org/downloads.html">Jython.jar</a> file in the 'Options' tab under 'Extender' in Burp Suite.
- Download the <a href="https://github.com/vsec7/BurpSuite-Xkeys/archive/master.zip">BurpSuite-Xkeys.zip</a>.
- In the 'Extensions' tab under 'Extender', select 'Add'.
- Change the extension type to 'Python'.
- Provide the path of the file "Xkeys.py" and click on 'Next'.

# Usage
- The extension will start identifying assets through passive scan.

## Result
- The extension will show on issues box and on output extender
<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/log.png">

## Possible Value Extraction
```
{keyword}=<value>
{keyword}= <value>
{keyword} =<value>
{keyword} = <value>
{keyword}'='<value>'
{keyword}'= '<value>'
{keyword}' ='<value>'
{keyword}' = '<value>'
{keyword}"="<value>"
{keyword}"= "<value>"
{keyword}" ="<value>"
{keyword}" = "<value>"
{keyword}":"<value>"
{keyword}": "<value>"
{keyword}" :"<value>"
{keyword}" : "<value>"
{keyword}=<value>&
```

## Requirements
- [Jython 2.7.0](https://www.jython.org/downloads.html)
- [Burp Suite Pro](https://portswigger.net/burp)

## Code Credits:
```
# PortSwigger example-scanner-checks: https://github.com/PortSwigger/example-scanner-checks
# Redhunlabs Asset_Discover: https://github.com/redhuntlabs/BurpSuite-Asset_Discover
```

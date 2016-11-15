# psc
Tiny little Script to read contents from "PodLove Simple Chapters" and display them as html

# Warning
I am not responsible for any harm this script does! Use at your own risk

## What it does
This script reads any *.PSC - file and displays the content as HTML in any Wordpress-Article

### Installation
#### Evil
Just copy the code into your theme's functions.php
(You will lose the script if you update/change your theme)

#### Good
1. Copy the "psc" - folder to wp-content/plugins
2. Activate it under "plugins"

### Configuration
There are three variables at the top of the file:
 $pscClass="entry-meta";
 $pscHeader="Pingbacks:";
 $pscUrlsOnly=true;

```php
$pscClass
```
defines a CSS-class that is wrapped around the DIV containing your information
```php
$pscHeader
``` 
is the Header-Text above your PSC-Content

```php
$pscUrlsOnly
```
if *true*: Displays only entries that have an url. 
If *false*: Displays all entries

### Usage
Insert `[PSC]yourUrl[/PSC]`at any place into your article.
Example: `[PSC]http://cdn.podseed.org/blathering/blathering_008.psc[/PSC]`

After saving, your Tag should be gone and be replaced by the content.

### Errors
If any error occurs (e.g. wrong filename), this should be displayed at the [PSC]-Position

### Easy-Installation-PlugIn
You won't find this PlugIn on Wordpress. You have to configure the vars and should know what you do. That's why there is no One-Click-Installation :)



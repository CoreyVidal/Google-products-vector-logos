# Google products vector logos  
A collection of only the highest quality and most accurate icons for various Google products.  


## Validation  
#### W3C SVG Validator  
SVGs must be validated by W3C Markup Validation Service:  
https://validator.w3.org/  
  
#### Wikimedia Commons SVG Validator  
SVGs must be validated by Wikimedia Commons SVG Checker:  
https://commons.wikimedia.org/w/index.php?title=Commons:Commons_SVG_Checker&withJS=MediaWiki:CommonsSvgChecker.js  
  
## Requirements  
#### Character Encoding  
Character encoding shall be declared at the document level.  
_Line 1, Column 1_: `<?xml version="1.0" encoding="utf-8"?>`  
  
#### SVG Document Structure  
SVGs shall be structured as follows:  
_Line 2, Column 1_: `<svg version="1.1" id="Content" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="192px" height="192px" viewBox="0 0 192 192" enable-background="new 0 0 192 192" xml:space="preserve">`  
  
#### Embedded Images  
SVGs must not contain embedded image rasters.  
###### Example:  
`<image xlink:href="data:image/png;base64,iVBORw0KGgoAAAElFTkSuQmCC" />`  
  
## Wikimedia Resources  
https://commons.wikimedia.org/wiki/Help:Illustrator  

## Editing in Adobe Illustrator (.ai)  
Artboard (Adobe Illustrator) should be 192 x 192px  
Artboard should start at the bottom-left (or top-left?) with coordinates 0,0  
Artboard should be named after the product icon. Example: "Google Maps"  
Root layer name should be "Content"  
Remove all other custom layer names  
Swap any layer that uses Fill Opacity to regular Opacity  
Replace any \<image\> layers with SVG Filters  
Make sure to use only one instance of material-drop-shadow  
  
## Exporting from Adobe Illustrator (.svg)  
File > Export > Export for Screens...  
* Format = SVG  
  
Format Settings > SVG:  
* Styling: Inline Style  
* Font: Convert To Outlines  
* Images: Embed  
* Object IDs: Layer Names  
* Decimal: 5  
* Minify: ☑  
* Responsive: ☑  
  
## After Exporting from Illustrator  
Open in Visual Studio Code  
Toggle Word Wrap: Alt + Z  
Format Document: Alt + Shift + F  
Replace/update lines 1 and 2  
Remove `name="material-drop-shadow"`  
Check there's no floating point errors  

## Replacing existing media
On Wikimedia Commons, check https://commons.wikimedia.org/wiki/Special:GlobalUsage

## Uploading
https://commons.wikimedia.org/wiki/Special:UploadWizard  


Creative Commons CC0 Waiver (release all rights, like public domain: legal code)

#### Image title
Google ______ icon

#### Caption
Product icon for Google ______


#### Description
This is the official product icon/logo for Google ______. It follows Google's Material Design guidelines: https://material.io/design/iconography/product-icons.html


#### Categories  
Google logos, Google SVG logos, Google software, Material Design product icons



#### Google Keep example

```
=={{int:filedesc}}==
{{Information
|description={{en|1=This is the official product icon/logo for Google Keep. It follows Google's Material Design guidelines: https://material.io/design/iconography/product-icons.html}}
|date=2013-03-20
|source=https://cloud.google.com/images/icons/ic_keep_24dp.svg
|author=Google LLC<br />SVG by [[User:CoreyVidal|CoreyVidal]]
|permission=
|other versions=
|other fields={{Igen|Adobe|+|s=tl}}
}}

=={{int:license-header}}==
{{PD-textlogo}}
{{Trademarked}}

[[Category:Google logos]]
[[Category:Google SVG logos]]
[[Category:Google software]]
[[Category:Material Design product icons]]
```

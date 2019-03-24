# Google products vector logos  
A collection of only the highest quality and most accurate icons for various Google products.  


### Validation  
#### W3C SVG Validator  
SVGs must be validated by W3C Markup Validation Service:  
https://validator.w3.org/  
  
#### Wikimedia Commons SVG Validator  
SVGs must be validated by Wikimedia Commons SVG Checker:  
https://commons.wikimedia.org/w/index.php?title=Commons:Commons_SVG_Checker&withJS=MediaWiki:CommonsSvgChecker.js  
  
### Requirements  
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
  
#### Tips from Wikimedia Commons  
https://commons.wikimedia.org/wiki/Help:Illustrator  
  
## Products  
  
#### Google Keep  
Wikimedia file: https://commons.wikimedia.org/wiki/File:Google_Keep_icon.svg  
Wikidata item: https://www.wikidata.org/wiki/Q7854718  
Wikipedia file: https://en.wikipedia.org/wiki/File:Google_Keep_icon.svg  
Wikipedia article: https://en.wikipedia.org/wiki/Google_Keep  

Original Wikipedia image: https://en.wikipedia.org/wiki/File:Google_Keep_icon.png  
Original Wikimedia image: https://commons.wikimedia.org/wiki/File:Google_Keep.jpg  

###### Changes  
`{{Vector version available|Google Keep icon.svg}}`
  . . _(Google Keep.jpg >> Google Keep icon.svg)_

###### Source  
Source file: https://cloud.google.com/images/icons/ic_keep_24dp.svg  
Source page: https://cloud.google.com/products/#g-suite  


## Editing in Adobe Illustrator (.ai)  
Artboard (Adobe Illustrator) should be 192 x 192px  
Artboard should start at the bottom-left (or top-left?) with coordinates 0,0  
Remove all custom layer names  
Swap any layer that uses Fill Opacity to regular Opacity  
Replace any <image> layers with SVG Filters  
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

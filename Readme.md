# Color Contrast Analyser for Sketch

A Sketch plugin that calculates the color contrast of two layers and evaluates it against the WCAG. If only a single layer is selected, than it will calculate with its artboard background color. The test may pass AAA, AA or fail because of a lack of contrast. And even when you do not need to meet those requirements, you can get a feeling for the contrast when you get used to the values. This might help you design accessible content.

![Screenshot](https://github.com/getflourish/Sketch-Color-Contrast-Analyser/raw/master/Sketch-Color-Contrast.png)

### AA requirements
Color contrast of **4.5:1** or **3.0:1 for large text**

### AAA requirements
Color contrast of **7.0:1** or **4.5:1 for large text**.

### A note on rounding (as of 21 Feb 2020)
The displayed values are not rounded, but limited to display two decimals. For example, a calculated contrast ratio of `1.39999` will be returned as `1.39` and won’t be rounded to `1.40`. This avoids false positives. 

## A note on "large" text
The WCAG specification of font size is given in CSS points. Those are not equal to the point size in Sketch. Text in Sketch is smaller than its CSS equivalent. Thus, the font size thresholds from the WCAG specification are converted to provide correct results in Sketch. 

Illustration:
https://codepen.io/getflourish/pen/oEyZRy

Details in Note 1: 
https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html

## Notes
- **Large text** means a font size of at least 24pt regular (18pt in CSS) or 18,66pt bold (14pt in CSS).  [Further details can be found in the Web Content Accessibility Guidelines 2.0.](http://www.w3.org/WAI/WCAG20/quickref/#qr-visual-audio-contrast-contrast)
- This plugin works with solid text and fill colors. Transparency is not supported yet. Version with transparency support can be found here: https://github.com/auxdesigner/Sketch-Color-Contrast-Analyser
- Calculations are based on [these color contrast algorithms.](http://gmazzocato.altervista.org/colorwheel/algo.php)

## Credits
Made by Florian Schulz ([@getflourish](https://twitter.com/getflourish) on Twitter), 2014

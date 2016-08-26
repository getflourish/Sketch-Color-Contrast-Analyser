# Color Contrast Analyser for Sketch

A Sketch plugin that calculates the color contrast of two layers and evaluates it against the WCAG. If only a single layer is selected, than it will calculate with its artboard background color. The test may pass AAA, AA or fail because of a lack of contrast. And even when you do not need to meet those requirements, you can get a feeling for the contrast when you get used to the values. This might help you design accessible content.

<img src="./Sketch-Color-Contrast.png" width="450px" alt="Sketch Color Contrast"" />

### AA requirements
Color contrast of **4.5:1** or **3.0:1 for large text**

### AAA requirements
Color contrast of **7.0:1** or **4.5:1 for large text**.

##Notes
- **Large text** means a font size of at least 18pt regular or 14pt bold. [Further details can be found in the Web Content Accessibility Guidelines 2.0.](http://www.w3.org/WAI/WCAG20/quickref/#qr-visual-audio-contrast-contrast)
- This plugin works with solid text and fill colors. Transparency is not supported yet. 
- Calculations are based on [these color contrast algorithms.](http://gmazzocato.altervista.org/colorwheel/algo.php)


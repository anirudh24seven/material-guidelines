## Typography
Since the Ice Cream Sandwich release, Roboto has been the standard typeface on Android. Since Froyo, Noto has been the standard typeface on Android for all languages not covered by Roboto. Noto is also the standard typeface for all languages on Chrome OS.

### Language categorization
Language scripts can be divided into three categories:

1. English and English-like: Latin (except Vietnamese), Greek, and Cyrillic scripts, supported by both Roboto and Noto. Roboto has been extended to completely cover all Latin, Greek, and Cyrillic characters as defined in Unicode 7.0. The number of supported characters has doubled from previous releases, from about 2000 to about 4000 characters
2. Tall: Language scripts that require extra line height to accommodate larger glyphs, including South and Southeast Asian and Middle-Eastern languages, like Arabic, Hindi, Telugu, Thai, Vietnamese. Noto supports these languages with two weights.
3. Dense: Language scripts that require extra line height to accommodate larger glyphs, including Chinese, Japanese, and Korean. Noto supports these languages with seven weights.

### Typeface
1. Roboto
  1. Roboto has been refined extensively to work across the wider set of supported platforms. It is slightly wider and rounder, giving it greater clarity and making it more optimistic.
  2. Roboto font weights
    1. Roboto has six weights: Thin, Light, Regular, Medium, Bold, and Black.
2. Noto
  1. Noto’s vertical metrics are compatible with Roboto.
  2. Noto font weights
    1. Noto Sans CJK (Chinese, Japanese, and Korean) has seven weights: Thin, Light, DemiLight, Regular, Medium, Bold, and Black. The weight of Noto Sans CJK Regular is the same as Roboto Regular.
    2. Noto fonts for Thai, Devanagari, and all other major living languages have Regular and Bold weights.
3. Hinted fonts
  1. Hints are the instructions embedded in a font on how to modify (distort) a glyph to look better on low-resolution displays. As a tradeoff, a hinted font consumes more space than the unhinted version.
  2. Both Roboto and Noto have hinted and unhinted versions. Google recommends:
    1. Use the unhinted versions on Android and on Mac OS X, which doesn’t implement hints.
    2. Use hinted fonts on Chrome OS, Windows, and Linux.
4. Font stack
  1. For both Android and web properties, the font stack should specify Roboto, Noto, and then sans-serif.
  
### Styles
1. Too many type sizes and styles at once can wreck any layout. A typographic scale has a limited set of type sizes that work well together along with the layout grid.
2. These sizes and styles were developed to balance content density and reading comfort under typical usage conditions. Type sizes are specified with sp (scaleable pixels) to enable large type modes for accessibility.
3. English and English-like scripts
  1. Latin, Greek, and Cyrillic.
  2. The basic set of styles are based on a typographic scale of 12, 14, 16, 20, and 34.
  3. Across form factors, text that appears in the app bar should use the Title style, Medium 20sp.
  4. In certain scenarios, use the larger Subhead style instead of the smaller Body style. Some of those scenarios include when information is presented as small snippets or when titles are paired with lines of Body-styled text.
  5. Button style (Medium 14sp, all caps) is used for all buttons. Button text should be all caps in languages that have capitalization. For languages that don’t have capitals, consider using color text for flat buttons to make them stand out from normal text.
4. Dense scripts
  1. Chinese, Japanese, and Korean.
  2. Weight: Since Noto CJK has seven weights that match Roboto, use the same weight settings as English.
  3. Font size: For Title through Caption styles, the font size is 1px larger than that specified for English. For styles larger than Title, the English type size is suitable.
5. Tall scripts
  1. South and Southeast Asian and Middle Eastern languages, including Arabic, Hindi, and Thai.
  2. Weight: Use Regular weight, as Medium weight is unavailable in Noto. Google recommends avoiding Bold weight, based on feedback from native speakers that Bold is too heavy.
  3. Font size: For Title through Caption styles, font size is 1px larger than that specified for English. For styles larger than Title, the English type size is suitable.


### Line height
To achieve proper readability and appropriate pacing, line heights have been determined based on each style’s individual size and weight. Line wrapping only applies to Body, Subhead, Headline, and the smaller Display styles. All other styles should exist as single lines.

1. English and English-like scripts
2. Dense and tall scripts
  1. For all styles, line height is 0.1em larger than the English-like languages. English and English-like languages mostly use a portion of the em box, often the lower portion below the x-height. Chinese, Japanese, and Korean (CJK) ideographic characters use the entire em box. Characters in tall languages often have long descenders and/or ascenders. To achieve the same design intention as English for CJK and to avoid potential text clipping between two lines next to each other for tall languages, the line height needs to be larger than in English for tall and dense languages.

### Other typographic guidelines
1. Colors & contrast
  1. A text color that is too similar to the background color is hard to read. Text with too much contrast can also be hard to read. This is especially true of light-colored text against dark backgrounds.
  2. Text should maintain a minimum contrast ratio of at least 4.5:1 (calculated based on luminance values) for legibility. A ratio of 7:1 is preferred.
  3. These color combinations also consider contrast ratios for users who perceive color differently.
2. Large and dynamic type
  1. For the best user experience, use dynamic type instead of relying only on smaller type sizes or allowing truncation of larger-size text.
  2. Large type applied correctly can make apps more interesting, differentiate layouts, and help users to decode content quickly.
  3. Dynamic type enables large type when the length of the text in a layout is unknown. Dynamic sizes are selected from a typographic scale based on available space and letter size estimates.
3. Line breaking
  1. The images show best practices for line breaks.
4. Tracking and kerning
5. Line length 
  1. Consider this advice on readability and line length from the Baymard Institute:
    1. “You should have around 60 characters per line if you want a good reading experience. Having the right amount of characters on each line is key to the readability of your text.”
    2. "Too wide – if a line of text is too long, the user’s eye will have a hard time focusing on the text. This is because the length makes it difficult to get an idea of where the line starts and ends. Furthermore it can be difficult to continue from the correct line in large blocks of text.”
    3. "Too narrow – if a line is too short, the eye will have to travel back too often, breaking the reader’s rhythm. Too short lines also tend to stress people, making them begin on the next line before finishing the current one (hence skipping potentially important words).”
    
### Language categories reference

For ease of internationalization, Google has categorized languages into three categories: English and English-like; tall; and dense.

1. English and English-like: Latin (except Vietnamese), Greek, Cyrillic, Hebrew, Armenian and Georgian.
2. Tall: Language scripts that require extra line height to accommodate larger glyphs, including South and Southeast Asian and Middle Eastern languages, like Arabic, Hindi, Telugu, Thai, Vietnamese.
3. Dense: Language scripts that require extra line height to accommodate larger glyphs but have different metrics from tall scripts. Includes Chinese, Japanese, and Korean.

## Units and measurements

Some units have different meanings in different contexts. This chapter discusses the usage of device-independent pixels, scaleable pixels, as well as concepts like pixel density.

### Pixel density
1. The number of pixels that fit into an inch is referred to as “pixel density.” High-density screens have more pixels per inch than low-density ones. As a result, UI elements (such as a button) appear physically larger on low-density screens and smaller on high-density screens.
2. Dpi, or screen resolution, refers to the number pixels there are in a particular display.
3. dpi = screen width (or height) in pixels/screen width (or height) in inches

### Density-independent pixels (dp)
1. "Density independence" refers to the uniform display of UI elements on screens with different densities.
2. Density-independent pixels (pronounced “dips”) are flexible units that scale to uniform dimensions on any screen. When developing an Android application, use dp to display elements uniformly on screens with different densities.
3. A dp is equal to one physical pixel on a 160-dpi screen. To calculate dp: dp = (width in pixels * 160)/dpi

### Scaleable pixels (sp)
1. When developing for Android, scaleable pixels (sp) serve the same function as dp, but for fonts. The default value of an sp is the same as the default value for dp.
2. The primary difference between an sp and a dp is that sp preserves a user's font settings. Users who have larger text settings for accessibility will see the font size matched to their text size preferences.

### Designing layouts for dp
1. When designing layouts for the screen, calculate an element’s measurements in dp: dp = (width in pixels * 160)/dpi
2. For example, a 32 x 32 px icon at 320 dpi equals 16 x 16 dp.

### Image scaling
Images can be scaled to look the same across different screen resolutions by using these ratios:

1. xxxhdpi: 4.0
2. xxhdpi: 3.0
3. xhdpi: 2.0
4. hdpi: 1.5
5. mdpi: 1.0

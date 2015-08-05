## Icons

### Product icons
1. Product icons are the visual expression of a brand’s products, services, and tools. Simple, bold, and friendly, they communicate the core idea and intent of a product. While each product icon is visually distinct, all product icons for a given brand should be unified through concept and execution.
2. Product icons are an essential vehicle for communicating your brand. Using these guidelines as a starting point, make sure your product icon colors and other key elements reflect your brand identity.
3. Design approach
  1. Product icon design is inspired by the tactile and physical quality of material. Each icon is cut, folded, and lit as paper would be, but represented by simple graphic elements. The quality of the material is sturdy, with clean folds and crisp edges. The matte-like finish interacts with light through subtle highlights and consistent shadows.
4. Product icon grid
  1. The product icon grid has been developed to facilitate consistency and establish a clear set of rules for the positioning of graphic elements. This standardization results in a flexible but coherent system.
5. Keyline shapes
  1. Keyline shapes are the foundation of the grid. By using these core shapes as guidelines, you can maintain a consistent visual proportion across related product icons.
6. DP unit grid
  1. Android expects product icons to be provided at 48dp, with edges at 1dp. When you create the icon, maintain the 48-unit measure, but scale it to 400% at 192 x 192 dp (the edge becomes 4dp).
  2. Any scaling done to the original will scale the image up or down proportionally. By maintaining the unit ratio, you preserve sharp edges and correct alignment when the scale is reduced.
7. Geometry
  1. Preset standards have been determined for specific keylines: circle, square, rectangle, orthogonals, and diagonals. This small palette of universal and simple elements has been developed to unify product icons and systemize their placement on the grid.
8. Product icon anatomy
  1. Product icon anatomy describes the graphic elements that make up a product icon. The consistency of these elements across icons for a given brand is critical in maintaining a shared visual language. Familiarity with these elements makes it easier to understand characteristics of each logo and subtle differences between them. It will also help educate your eye to recognize the underlying structure of logo designs.
    1. Finish
    2. Material background
    3. Material foreground
    4. Color
    5. Shadow
9. Product icon metrics
  1. Lighting
    1. Within the material environment, virtual lights illuminate the scene and allow objects to cast shadows. A top light cast on material elements creates a contact shadow while highlighting the top and bottom edges. An angled light reinforces the sense of surface across the elements.
  2. Shadows
    1. For a product icon, the top light from above casts a soft shadow surrounding an element lightly on the top and left. The shadow is slightly heavier below and to the right. This shadow is always contained within the icon’s silhouette.
  3. Edge tint and shade
    1. The top and bottom edges of material elements provide a sense of depth and surface. Material elements have a standard 1dp thickness. All edge distances are measured from an element's interior edge. 
    2. Tint highlights the top edge of all elements. The left, right, and bottom edges do not have a tint applied. 
    3. Shade darkens the bottom edge of all elements. The left, right, and top edges do not have a shade applied.
  4. Finish
    1. The finish layer is a result of the virtual 45º light source. It extends from the top-left corner to the exterior edge of the icon’s silhouette. The finish is always contained within these boundaries.
  5. Tint, shade, and shadow values
    1. Each color reacts differently when tints and shades are added. The color of every edge tint, edge shade, and shadow needs to be adjusted for each color that lies behind it. To ensure color harmony, follow the appropriate value for each.
10. Product icon patterns
  1. Influenced by the behavior of physical material, simple conventions provide a sense of surface and tactility. The interactions of material and color allow for numerous unique compositions.
  2. Color
    1. Color elements are flush to the paper’s surface.
    2. Don’t embellish color elements with any edges or shadows.
  3. Layer
    1. Layered paper elements create depth, having edges and shadows.
    2. Be cautious with the quantity of overlapping surfaces. Having too many complicates the icon and lacks focus.
  4. Elevate
    1. Elevating a key material element atop a simple background silhouette focuses attention to the center.
    2. Don’t crop elevated material elements within another shape.
  5. Score
    1. Scored material elements have the illusion of depth without losing their geometric form. Scores should be centered on symmetrical shapes.
    2. Don’t use multiple scores, or position a score off-center.
  6. Fold
    1. Folded material elements are skewed, having greater dimension. Spot colors should be avoided, so as to avoid altering or misrepresenting key elements.
  7. Overlap
    1. Overlapped material elements create unique silhouettes. All elements, edges, and shadows are confined to the interior of the silhouette.
    2. Don’t exceed more than two overlaps. Having too many complicates the icon and lacks focus.
  8. Accordion
    1. Accordion folded material elements are adjoined by a connecting fold, used to add dimension to a single material element.
    2. Don’t exceed more than two accordion folds. Having too many complicates the icon and lacks focus.
  9. Distort
    1. Product icons should never be distorted or transformed. Elements should remain in their geometric form, and not be skewed, rotated, bowed, warped, or bent.
11. Human iconography: The below guidelines and examples illustrate best practices for incorporating human iconography into your UI.
  1. Form
  2. Keyline shapes
  3. Paper vs color
  4. Gestures
  5. Human icon rules

### System icons
1. A system icon, or UI icon, symbolizes a command, file, device, or directory. System icons are also used to represent common actions like trash, print, and save.
2. The design of system icons is simple, modern, friendly, and sometimes quirky. Each icon is reduced to its minimal form, with every idea edited to its essence. The designs ensure readability and clarity even at small sizes.
3. Design principles
  1. Shapes are bold and geometric.
  2. Symmetry and consistency of shapes give the icons a unique quality, while keeping them simple and bold.
4. Grid, proportion, and size
  1. DP unit grid
    1. System icons are displayed at 24dp. When creating icons, it’s important to design at 100% scale for pixel-accuracy, while zooming in for precision.
  2. Icon grid
    1. The icon grid has been developed to facilitate consistency and establish a clear set of rules for the positioning of graphic elements. This standardization results in a flexible but coherent system.
  3. Content area
    1. The content of an icon should remain inside of the live area. Content should only extend into the trim area if additional visual weight is needed. Do not place any part of the icon outside of the trim area.
  4. Keyline shapes
    1. Keyline shapes are the foundation of the grid. By using these core shapes as guidelines, you can maintain a consistent visual proportion throughout the system icons.
  5. Geometry
    1. Preset standards have been determined for specific keylines: circle, square, rectangle, orthogonals, and diagonals. This small palette of universal and simple elements has been developed to unify Google system icons and systemize their placement on the icon grid.
  6. System icon anatomy
    1. Stroke terminal
    2. Corner
    3. Counter area
    4. Stroke
    5. Counter stroke
    6. Bounding area
  7. Corners
    1. Consistent corner radiuses are key to unifying the overall system icon family. A 2dp corner radius is used on the silhouette form of the icon. Do not round the corners of strokes (shapes 2dp wide or less).
    2. Interior corners should be square. Do not round the corners of interior shapes.
  8. Strokes
    1. Consistent stroke weights are key to unifying the overall system icon family. Maintain a 2dp width for all stroke instances, including curves, angles, and both interior and exterior strokes.
  9. Optical corrections
    1. Extreme scenarios that call for subtle tweaks add to the legibility of an icon. Instances where complex details are unavoidable require adjusting metrics.
    2. If optical corrections are necessary, only use the consistent geometric forms on which all other icons are based. Don’t skew or distort the forms.
  10. Clearance
    1. Adequate space around the icon is needed to allow for legibility and touch.  
  11. Best practices
    1. Consistency aids user comprehension of icons. Use the existing system icons whenever possible and across different applications.
5. Human iconography
  1. Human icon anatomy
    1. Head
    2. Neck
    3. Upper body
    4. Arm
    5. Leg
  2. Form
  3. Full body
  4. Upper body
  5. Contained
  6. Detailed parts
  7. Human icon rules
6. Color
  1. The standard opacity for an active icon on a light background is 54% (#000000). An inactive icon, which is lower in the visual hierarchy, should have an opacity of 26% (#000000).
  2. The standard opacity for an active icon on a dark background is 100% (#FFFFFF). An inactive icon, which is lower in the visual hierarchy, should have an opacity of 30% (#FFFFFF).

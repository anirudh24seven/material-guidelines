## Material properties
Material has certain immutable characteristics and inherent behaviors. Understanding these qualities will help you manipulate material in a way that’s consistent with the vision of material design.

### Physical properties
1. Material has varying x & y dimensions (measured in dp) and a uniform thickness (1dp).
2. Material casts shadows. Shadows result naturally from the relative elevation (z-position) between material elements.
3. Content is displayed on material, in any shape and color. Content does not add thickness to material.
4. Content can behave independently of the material, but is limited within the bounds of the material.
5. Material is solid. Input events cannot pass through material.
6. Multiple material elements cannot occupy the same point in space simultaneously.
7. Material cannot pass through other material. For example, one sheet of material cannot pass through another sheet of material when changing elevation.

### Transforming material
1. Material can change shape.
2. Material grows and shrinks only along its plane.
3. Material never bends or folds.
4. Sheets of material can join together to become a single sheet of material.
5. When split, material can heal. For example, if you remove a portion of material from a sheet of material, the sheet of material will become a whole sheet again.
6. 

### Movement of Material
1. Material can be spontaneously generated or destroyed anywhere in the environment.
2. Material can move along any axis.
3. Z-axis motion is typically a result of user interaction with material.

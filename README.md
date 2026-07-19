# Echo Crystal Cavern

## Project Description

Echo Crystal Cavern is a small fantasy environment created in Unreal Engine 5. The project focuses on creating a visually immersive cave using physically based materials, shaders, lighting, and atmospheric effects. Players explore a hidden cavern illuminated by glowing crystals and surrounded by detailed rock formations.

---

## Initial Project Setup

1. Created a Blank Unreal Engine 5 project.
2. Added Starter Content.
3. Created the main cave level.
4. Added placeholder cave meshes and lighting.
5. Organized project folders for Materials, Meshes, Textures, Blueprints, and Maps.
6. Initialized Git version control.
7. Connected the project to GitHub.
8. Added an Unreal Engine `.gitignore` file.
9. Pushed the initial project to GitHub.
10. Added the instructor as a collaborator.

---

## Topic 2: Basic Shader Creation

For this milestone, I created a custom crystal shader using the Unreal Engine Material Editor.

### Material Name

`M_CrystalGlow`

### Shader Features

- Adjustable crystal color using a Vector Parameter.
- Fresnel edge glow effect.
- Adjustable emissive intensity using a Scalar Parameter.
- Bright glowing crystal appearance.

### Shader Creation Process

1. Created a new material named `M_CrystalGlow`.
2. Added a Vector Parameter named `CrystalColor`.
3. Connected the color to the Base Color input.
4. Used a Fresnel node to create edge highlighting.
5. Multiplied the Fresnel effect with the crystal color.
6. Added a Scalar Parameter named `GlowIntensity`.
7. Connected the result to the Emissive Color input.
8. Applied the material to the crystal meshes in the scene.

### Challenges

One challenge was controlling the brightness of the emissive glow. At first the crystal appeared too bright, making it difficult to see surface details. Creating a GlowIntensity parameter allowed me to easily adjust the brightness until it looked more natural.

---

## Topic 3: Physically Based Materials (PBR)

For this milestone, I created a physically based rock material to improve the realism of the cave environment.

### Material Name

`M_CaveRock_PBR`

### PBR Textures Used

- Base Color (Albedo)
- Roughness
- Normal Map
- Ambient Occlusion

The rock material uses a Metallic value of 0 because natural stone is not metallic.

### Normal Mapping

A normal map was applied to create the appearance of cracks, bumps, and uneven rock surfaces without increasing the mesh complexity. This added much more detail to the cave walls while maintaining good performance.

### Lighting Improvements

To better showcase the material, I adjusted the cave lighting by placing colored lights near the crystal formations. The lighting highlights the rough stone surfaces and makes the normal map details more visible. These adjustments helped create a more immersive cave atmosphere.

### Challenges

One challenge was understanding how each PBR texture affected the final material. After experimenting with the albedo, roughness, ambient occlusion, and normal maps, I learned how each texture contributes to creating realistic surfaces. I also had to ensure the normal map was imported correctly so Unreal recognized it as a normal map rather than a regular image.

---

## Reflection

Working with shaders and PBR materials helped me better understand how materials are built inside Unreal Engine. Before this project I mainly viewed materials as simple textures, but I now understand how multiple texture maps and material nodes work together to create realistic surfaces. I also became more comfortable using the Material Editor and troubleshooting connections between different nodes.

---

## Future Plans

- Add animated crystal shaders.
- Improve cave lighting and atmosphere.
- Create a reflective water material.
- Add moss and wet rock variations.
- Continue refining the cave environment for the final project.

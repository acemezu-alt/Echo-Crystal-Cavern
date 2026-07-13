# Echo Crystal Cavern

## Project Description

Echo Crystal Cavern is a small fantasy environment created in Unreal Engine 5. The scene focuses on glowing crystal formations, cave surfaces, atmospheric lighting, and environmental shader effects.

## Initial Project Setup

1. Created a Blank Unreal Engine 5 project.
2. Enabled Starter Content.
3. Created the main crystal cavern level.
4. Added placeholder cave walls, rocks, lighting, and crystal meshes.
5. Organized the project into folders:
   - Materials
   - Material Instances
   - Meshes
   - Textures
   - Blueprints
   - Maps
6. Initialized Git version control.
7. Connected the local project to GitHub.
8. Added an Unreal Engine .gitignore file.
9. Pushed the initial project setup to the repository.
10. Added the instructor as a repository collaborator.

## Topic 2 Shader Development

For this stage of the project, I created a basic glowing crystal shader using the Unreal Engine Material Editor.

### Material Name

M_CrystalGlow

### Shader Features

- Adjustable crystal color
- Emissive glow
- Fresnel-based edge lighting
- Adjustable glow intensity
- Optional pulsing animation
- Subtle moving surface pattern

### Shader Creation Process

1. Created a new material named M_CrystalGlow.
2. Added a Vector Parameter named CrystalColor.
3. Connected CrystalColor to the Base Color input.
4. Used a Fresnel node to create stronger lighting around the edges of the crystal.
5. Multiplied the Fresnel effect by CrystalColor.
6. Added a Scalar Parameter named GlowIntensity.
7. Connected the final result to Emissive Color.
8. Added a Time and Sine node to create a subtle pulsing glow.
9. Used Texture Coordinate and Panner nodes to create movement across the crystal surface.
10. Applied the material to a crystal mesh in the scene.
11. Created a Material Instance for easier customization.

## Challenges and Solutions

One challenge was controlling the brightness of the emissive effect. At first, the crystal appeared either too dark or extremely bright. I solved this by creating a Scalar Parameter for the glow intensity, which allowed me to adjust the brightness more easily.

Another challenge was making the pulsing effect subtle. The original animation changed too quickly and distracted from the environment. I reduced the Time multiplication value to slow the animation and used a Sine node to create a smoother transition.

I also had to make sure the moving texture effect did not look too fast or repetitive. Lowering the Panner speed helped create a slower and more natural-looking effect.

## Personal Reflection

Creating this shader helped me better understand how different material nodes work together. Before this assignment, I mainly thought of materials as static textures. I now understand that materials can use mathematical values, parameters, and time-based nodes to create dynamic visual effects.

The Material Editor made shader creation feel more approachable because I could visually connect nodes and immediately preview the results. This process also taught me the importance of testing small changes instead of adding too many effects at once.

## Future Plans

- Create additional crystal color variations.
- Improve the crystal surface texture.
- Add wet rock materials.
- Create a reflective cave-water shader.
- Improve lighting and atmospheric fog.
- Optimize the materials for performance.

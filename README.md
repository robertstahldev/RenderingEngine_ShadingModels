Shading Models and Rendering Optimization

Project Overview

  This project was created in Unity 6.6 using the Universal Render Pipeline (URP). The purpose was to explore how different shading models affect the appearance of 3D objects and how rendering optimization can improve efficiency.

Scene and Features
  The scene includes several primitive shapes, including cubes, spheres, capsules, cylinders, and planes, along with a floating island model I previously created in Blender.
  I experimented with Unlit and Lit materials, metallic and smoothness properties, and a custom toon shader created using Shader Graph.
  I also applied a PNG texture I created for an earlier assignment to a cube to demonstrate how textures provide colors and patterns, while shaders determine how those colors respond to lighting.

Rendering Optimization
  I tested GPU instancing using 48 identical spheres.
  Before enabling GPU Resident Drawer instancing, Unity's Profiler reported 658 draw calls. After enabling instancing, that decreased to 374 draw calls, approximately a 43.2% reduction.
  SetPass calls remained at 34, and the triangle and vertex counts remained unchanged. I also used Unity's Frame Debugger to verify that instanced rendering was occurring.

How to Open the Project
  -Clone or download this repository.
  -Open Unity Hub and select Add Project.
  -Select the downloaded project folder.
  -Open the project using Unity 6.6.
  -Open the main scene from the Assets folder.
  -Press Play to run the scene, or inspect the materials and shaders directly in the Unity Editor.

Loom Video
https://www.loom.com/share/480e5547866a4ef5a92f2a13a9d239e1

Screenshots
<img width="481" height="278" alt="TexturedCubeLowLight" src="https://github.com/user-attachments/assets/62f0382c-0362-4478-bbbb-ef088bd8fc01" />
<img width="383" height="301" alt="TexturedCubeLight" src="https://github.com/user-attachments/assets/6cbd8f91-d185-45bc-9824-11be1e0c7a35" />
<img width="409" height="349" alt="TexturedCubeDark" src="https://github.com/user-attachments/assets/4b2b2939-a84d-46b6-8abf-0f8e11c6669c" />
<img width="634" height="782" alt="ProfilerInstanced" src="https://github.com/user-attachments/assets/a195746b-7c80-46f8-9737-862d51c59174" />
<img width="991" height="498" alt="ProfilerHybridBatch" src="https://github.com/user-attachments/assets/85b2e63e-ed9b-4968-8f17-9be27816ccc7" />
<img width="656" height="837" alt="ProfilerBaseline" src="https://github.com/user-attachments/assets/e108064d-8470-488d-b4e0-3419eebb23bd" />
<img width="222" height="247" alt="MetallicView_EnviroOff" src="https://github.com/user-attachments/assets/3af7380b-8899-43e0-bcae-357f58c50d82" />
<img width="170" height="198" alt="MetallicView" src="https://github.com/user-attachments/assets/3ab8f020-58f6-4a63-bc71-ce1d2528753e" />
<img width="365" height="618" alt="CartoonMaterial" src="https://github.com/user-attachments/assets/04d2d802-9719-48d2-a4f0-dbd18e397291" />
<img width="550" height="593" alt="Cartoon_TwoTone" src="https://github.com/user-attachments/assets/f1e0f1d6-e5e5-44cb-88f0-2a32d331cf10" />

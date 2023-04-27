
# 📃 About me
Self-motivated and highly curious Software Engineer with a strong aptitude for problem-solving and a passion for continuous learning. 
Proficient in various programming languages and software development methodologies. Demonstrated success in delivering innovative and effective solutions for a diverse range of projects.


___
# ⚒️ Projects
## Timer Module and Profiler — [Repo](https://github.com/syn-chromatic/timer-module)
A Python project that combines a timer module and a custom profiler to analyze and optimize the performance of your code. The timer module helps track the execution time of specific code blocks, while the custom profiler provides insights into the function calls and their performance. This combination of tools makes it easier to identify bottlenecks, and improve the efficiency of your code.


## Levenshtein Algorithm — [Repo](https://github.com/syn-chromatic/levenshtein-distance)
A Python project that implements the Levenshtein distance algorithm to measure the similarity between two strings. The algorithm calculates the minimum number of single-character edits (insertions, deletions, or substitutions) required to transform one string into another. This efficient and versatile algorithm has applications in fields such as natural language processing, data cleansing, and spell checking.


## Discord Bot Automatic Background Removal — [Repo](https://github.com/syn-chromatic/discord-bg-removal-bot)
A powerful tool that leverages machine learning to seamlessly remove backgrounds from images and videos. For videos, it deconstructs them into frames, processes each frame individually, and reconstructs the video with the background removed without requiring any input from the user to outline the background, which makes it a perfect fit for a Discord Bot.


## Custom Game Engine — [Repo](https://github.com/syn-chromatic/rust-g-engine)
Initially intended as an exploration into game development and related concepts, this quickly evolved into a passion-driven project of mine.

### 🎥 Camera Projection
Grasping the concept of camera projection proved challenging at first.
Imagine you have a virtual world within a cube, where for each axis of this world is the maximum floating-point that a computer can represent, now imagine you want to set up a view point and look through this world.



| matrix representation of a world  |
| :---: |
| <img src="https://github.com/syn-chromatic/syn-chromatic/blob/main/media/world.png"/> |


One might assume it'd be as simple as viewing the world through one side and displaying everything on screen, but this is an inaccurate representation of 3D perception for key reasons:

If we flatten the Z-Axis onto a 2D plane, which is fundamentally the same idea as looking through this world from one of its sides

| flattened world |
| :---: |
| <img src="https://github.com/syn-chromatic/syn-chromatic/blob/main/media/flattened_world.png"/> |


This suddenly creates a problem, if you imagine those two particles moving away from you in a parallel path, meaning that the distance between them stays the same, then through that same view, it would appear as the particles are keeping the same distance, because it is linearly defined in this world, but that's not how 3D perception works, the particles should appear closer together as they move away.

This is where camera projection comes in, by creating a virtual frustum, we can define two planes (Near Plane and Far Plane) and intersect the objects that are present inside.

| camera frustum |
| :---: |
| <img src="https://github.com/syn-chromatic/syn-chromatic/blob/main/media/frustum.gif"/> |

### 💥 Physics 
Physics presents a significant challenge in game development due to processing limitations and the need to balance realistic physics with interactivity. This often necessitates making trade-offs in performance and accuracy.

#### Main Types of Collision Detection 
##### Discrete Collision Detection 
The most direct approach involves updating an object's position at each timestep of the physics simulation. However, this method can lead to objects moving too quickly, phasing through walls without detection.

| discrete collision |
| :---: |
| <img src="https://github.com/syn-chromatic/syn-chromatic/blob/main/media/discrete_collision.png"/> |


##### Continous Collision Detection 
This method is similar to discrete detection but calculates potential collisions ahead of time based on an object's trajectory, and interpolating the potential positions of the object between time steps, this is computationally expensive, but it provides high accuracy.


| continous collision |
| :---: |
| <img src="https://github.com/syn-chromatic/syn-chromatic/blob/main/media/continous_collision.png"/> |



### Engine Preview
While numerous challenges and problems remain, the project has made significant progress. Here are a few examples showcasing the engine's current state

#### Soft Lighting Without Textures  
https://user-images.githubusercontent.com/68112904/234850939-4f99d88a-4ecb-4c43-9965-f04b89f3aef1.mp4


#### Physics
https://user-images.githubusercontent.com/68112904/234851105-d1793137-a2b5-41d9-aa65-d89482aa5aea.mp4


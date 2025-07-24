# Demo-Computer-Graphics
Demonstration of project computer graphics moved from school's private repository to public personal repository.

# About
This project showcases a demo of a minecraft terrain genrator in JavaScript with Webgl.

# Setup

- Download the entire project and open with visual studio code
- Install the extension "Live Server"
- Right click on index.html and choose the option "Open with live server"

# How it works 

### Buffer.js
Defines the shape of a cube 
- Creates the 3D coordination for cube corners
- Sets up texture coordinates
- Defines surface normals

### shader.js
contains the graphics shaders
- Vertex Shaders: Determines position of every cube in 3D world space
- Frag,emt Shaders Determines colors of each piuxel, applies texture and lighting.

### texture.js
loads images to put on cube faces
- Loads png files

### Perlinnoise.js
creates natural random patterns
- generate terrain heights
- makes hills and valleys not completely random

### main.js
Setup phase
- Webgl initialization
- Shader compilation
- Buffer creation
- texture loading

World generation

- Use perlin noise to create hills
- Each colujmn gets a height based on smooth random values
- Place different block types at different depths

Tree generation

- Randomly places trees on grass blocks
- Each tree has a wood trunk and leaf crown

Cave generation

- Creates a worl-like cave that tunnel through the terrain
- removes block along the paths to create hollow spaces 


# Showcase

<img width="1908" height="912" alt="image" src="https://github.com/user-attachments/assets/ac1781fb-431e-43e0-8655-ac7e61a36ba0" />

### each refreshed page is a newly generated terrain

<img width="1906" height="916" alt="image" src="https://github.com/user-attachments/assets/b37e1085-0b42-4ec9-87e7-4c1415775c8d" />

### can also change terrain width and length 

<img width="1899" height="905" alt="image" src="https://github.com/user-attachments/assets/12983071-cc37-4893-b52c-4ce0d1e1c4eb" />




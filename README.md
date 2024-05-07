how to use this app:
- drag with your mouse on the 3D area to rotate the camera
- left mouse button drag to pan the camera
- middle mouse button drag to zoom in/out
- click on the menu on the left to select an object category
- click on an object to add it to the scene
- use the red/green/blue arrows to move the object along the 3 axes
- use the keys Q (translate), W (rotate) and E (scale) or click on the buttons below the object menu to alternate the transform actions
- use the DEL key or the trash bin icon to delete objects
- click on the light bulb icon to add more lights to the scene
- once a light is placed, you can select it to change its intensity and color

You can modify the default scene by editing (or adding more files) the scene01 and scene02 JSON files inside the folder ./js:

[
    {"type": "object", "id": 6, "position": [-1.0,0,0], "rotation": [0,0,0], "scale": [1,1,1]},
    {"type": "object", "id": 11, "position": [-1.7,0,1.4], "rotation": [0,0,0], "scale": [1,1,1]},
    {"type": "object", "id": 25, "position": [-1.5,0,-1.4], "rotation": [0,0,0], "scale": [0.8,0.8,0.8]},
    {"type": "object", "id": 39, "position": [1.6,0,-1.55], "rotation": [0,-90,0], "scale": [1,1,1]},
    {"type": "object", "id": 39, "position": [0.85,0,-1.55], "rotation": [0,-90,0], "scale": [1,1,1]},
    {"type": "object", "id": 42, "position": [0,0,0], "rotation": [0,0,0], "scale": [4,1,4]},
    {"type": "object", "id": 41, "position": [-2.0,0,0], "rotation": [0,0,0], "scale": [1,1,4]},
    {"type": "object", "id": 41, "position": [0,0,-2.0], "rotation": [0,-90,0], "scale": [1,1,4]},

    {"type": "light", "position": [0,3,0], "intensity": 0.2, "color": "#0000ff"},
    {"type": "light", "position": [-1.5,1.4,-1.4], "intensity": 0.2, "color": "#f9f5b7"}
]

You can find the object IDs on the file params.json. There are two types of objects: object and light.

To use different scene default files, just edit the file name in the line 490:

fetch("./js/scene01.json")


And that's it! I hope you like it. We could implement other useful functions such as changing material colors and textures, adding different kinds of objects, such as procedural objects, and more.

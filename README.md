# MG5
## Devlog
Q1: 
A NavMesh makes more sense when the question is where a character should go. You give it a destination, and it finds a route around obstacles. Physics makes more sense when the question is how a character moves. NavMesh example: a Diablo-style action RPG. The player clicks a spot and the hero walks there, automatically steering around walls and pillars. Enemies also need to chase the player through winding dungeons. Physics example: Rocket League. Cars accelerate, jump, flip, drive up walls and collide with each other and the ball. The whole game comes from momentum and the exact angle and speed of each impact. 
Q2: 
Each time the loop runs, it takes one bird from the _birds array (_birds[i]) and checks whether that bird is close enough to the player to react. By the end of the loop, every bird has been checked once, and this repeats every frame because the loop is inside Update. What Vector3.Distance is used for: it takes two positions, here the bird’s and the player’s, and returns the straight-line distance between them in world units as a float.Which birds run away: only birds whose distance to the player is less than or equal to _interactDistance. 

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [Mountain fantasy environment models](https://www.fab.com/listings/60487a72-3f20-4bb2-aa78-247ed1582656)

# MG4
## Devlog

FloatAnimation makes an object bob up and down forever. Start() sets _timer to _switchSpeed (3 s) so the first leg is full length, while _up defaults to false, meaning it starts moving downward. Each frame, Update() moves the object along Y by _moveSpeed * Time.deltaTime, with the sign chosen by _up, then subtracts Time.deltaTime from _timer. When _timer hits zero, it resets to _switchSpeed and _up = !_up flips the direction, so the food descends for 3 seconds, ascends for 3 seconds, and repeats.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)

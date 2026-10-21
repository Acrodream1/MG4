# MG4
## Devlog

The way the floatAnimation script works is that the Start() method initializes the timer to equal the switchspeed which is used to track how long until the floating animation switches direction. In the Update() method, the timer is decreased every frame using deltatime smooth and accurate. The same thing is also applied to the food's position. The y position value of its transform is changed using Transform.translate with small increments using deltatime to make sure that the ball moves at the same rate in other refresh rates. Once the timer reaches 0, the direction of the animation is flipped by setting the _up variable to its opposite boolean value and the timer is set back to the switchtimer variable. This allows the floatAnimation of the food to repeat indefinitely until the food is collected.

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)
## Live update
For live-update development, install live-server first.
```
npm install -g live-server
```

then add scripts to package.json to run live-server.

## Basic Usage

If for some reason square stars bother you, you can use a custom image to replace the stars:

``` html
<a-entity star-system="texture: https://cdn.rawgit.com/matthewbryancurtis/aframe-star-system-component/master/assets/star.svg"></a-entity>
```
## Properties

The way this works is it creates a bunch of particles (stars) in THREE. The particles are randomly placed between two spheres: sphere of radius 'radius' and sphere of radius 'radius + depth'. You can also load a custom sprite to replace the squares that THREE.PointsMaterial() makes.

| Property    | Type   | Default | Description                                         |
|-------------|--------|---------|-----------------------------------------------------|
| color       | String | '#FFF'  | Color of the star particles                         |
| radius      | Number | 300     | Distance from center of sphere to inner star sphere |
| depth       | Number | 300     | Distance between inner sphere and outer sphere      |
| size        | Number | 1       | Size of each individual star                        |
| count       | Number | 10000   | Number of total stars created                       |
| texture     | Asset  | ''      | Sprite used for individual stars (ex: PNG image)    |

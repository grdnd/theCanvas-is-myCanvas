# Getting started with Three.js

## What is Three.js?

In order to understand `three.js`, we must first understand `WebGL`.

#### WebGL

**WebGL** performs as a `rasterizing engine` that draws points, lines, and triangles with the data received from a developer's code.

This `JavaScript API` gives devs the ability to render interactive 2D and 3D graphics directly within the web browser.

However, WebGL requires extensive lines of code to render even the simplest of 3D objects -- to make this process more practical, we now use three.js.

### Three.js

`three.js` is a JavaScript library _and_ API that streamlines the process of designing 3D graphics in the web browser by handling complex WebGL processes such as:

    | scenes
    | lights
    | shadows
    | materials
    | textures
    | 3D math

By reducing the time developers would have spent coding with WebGL native, three.js ultimately enables them investment in to more 3D projects and unsuppressed creative freedom.

## Getting Started

To begin developing in three.js, we must first create a document or `canvas` to accommodate our 3D objects.

For this exercise we will create an HTML file with the following code as our base:

```
| <!DOCTYPE html>
| <html>
|   <head>
|     <meta charset="utf-8">
|     <title>My first three.js app</title>
|     <style>
|       body { margin: 0; }
|     </style>
|   </head>
|   <body>
|     <script src="js/three.js"></script>
|     <script>
|       // Our Javascript will go here.
|     </script>
|   </body>
| </html>
```

## Retrieve Three.js Build

Once we have our HTML file set up, let's create the following javascript file-directory:

    /js/three.js

\*_This can be named however you like as long as your JavaScript is linked properly within the `script` tags of our HTML file._

Now, let's copy the three.js source code from their build website:

[Click here for three.js source code](https://threejs.org/build/three.js)

Paste the source code into our `three.js` file we just created and save.

## The 3 Requirements

In order for us to actually start displaying objects within our canvas, we must create 3 things:

**_Scene_** | **_Camera_** | **_Renderer_**

We can set this up simply by using javascript to declare our objects.

```
const scene = new THREE.Scene();

const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

const renderer = new THREE.WebGLRenderer();

renderer.setSize( window.innerWidth, window.innerHeight );

document.body.appendChild( renderer.domElement );
```

Although we have yet to see any visual changes, with these 3 objects we have now created an environment where we may render now 3D objects within our scene which is viewed from the camera.

### The Camera

Three.js comes with an assortment of `cameras` allowing developers to interact with their renders in different ways through the lens they choose.

```
| ArrayCamera

| Camera

| CubeCamera

| OrthographicCamera

| PerspectiveCamera

| StereoCamera
```

## Installation

## Usage

##

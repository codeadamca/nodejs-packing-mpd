# Converting LDR Files to Packed MPD Files

This repo stores the files and instructions to convert an `.ldr` file created using [BrickLink Studio](https://www.bricklink.com/v3/studio/download.page) to a packed `.mpd` file. This is the file type required by [THREE.js](https://threejs.org/) to display a [BrickLink Studio](https://www.bricklink.com/v3/studio/download.page) project in a web page.

For an example check out the [LDrawLoader documentation](https://threejs.org/docs/#examples/en/loaders/LDrawLoader) and [LDrawLoader examples](https://threejs.org/examples/#webgl_loader_ldraw). 

To convert your `.ldr` file, follow these steps:

1. Download and unzip the complete [LDraw Part Library](https://library.ldraw.org/updates?latest).
2. Move the `.ldr` file you want to convert to the `ldraw/models/` folder.
3. Download just the `packLDrawModel.mjs` object file from the [THREE.js](https://github.com/mrdoob/three.js/blob/master/utils/packLDrawModel.mjs) GitHub repo and place it in the `ldraw/` folder.
4. Your folder structure should look like this: 

  ```
  ├── ldraw
  │   └── models
  │   │   └── yourModel.ldr
  │   ├── p
  │   └── parts
  └── packLDrawModel.mjs
  ```

5. Open up the terminal, navigate to the `ldraw/` folder and run the following command:

  ```
  node packLDrawModel.mjs models/yourModel.ldr
  ```

  > [!NOTE]
  > Note: Replace `yourModel.ldr` with the name of your model.

6. You new file will be named `yourModel.ldr_Packed.mpd`.

---

## Project Stack

This project uses [Node.js](https://nodejs.org/en) and [THREE.js](https://threejs.org/).

<img src="https://console.codeadam.ca/api/image/nodejs" width="60"> <img src="https://console.codeadam.ca/api/image/threejs" width="60">

---

## Repo Resources

* [THREE.js]([https://www.brickmmo.com/](https://threejs.org/))
* [LDraw](https://ldraw.org/)

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>

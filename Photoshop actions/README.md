# Photoshop actions

## Important

These Photoshop actions are added to this repository, because the images are ultimately resized to different sizes for a personal project:
- 17x12 (@1x)
- 34x24 (@2x)
- 51x36 (@3x)

The actions include:
- A Save for Web export (legacy)
- A TinyPNG export, which depends on the [TinyPNG/JPG plugin](https://tinypng.com/photoshop) for Photoshop

## Limitations

**Note**: One of the limitations of Photoshop actions is that export paths are all absolute instead of relative. You may need to adjust the actions manually to edit export paths.

The current structure in the actions is:
- desktop
  - exports _(used in the 'Save for Web' action)_
    - 17x12
    - 34x24
    - 51x36
  - exports-tinypng _(used in the 'TinyPNG' action)_
    - 17x12
    - 34x24
    - 51x36

## Usage

1. Group all @3x exported images from the Sketch file in a new folder
2. Open Photoshop
3. In the menu, go to File > Automate > Batch
4. For 'Set', select 'FlagKit-UUID'
5. For 'Action', select the preferred export method
6. For 'Source', select 'Folder' and below that, choose the folder created in step 1
7. Press 'OK'. If successful (this depends if the absolute paths are fixed), the images are stored in the three sizes specified above, in separate folders.
8. _(If needed) Remove the '@3x' suffix from the exported files._

## License

FlagKit is released under the MIT license. See
[LICENSE](https://github.com/madebybowtie/FlagKit/blob/master/LICENSE).

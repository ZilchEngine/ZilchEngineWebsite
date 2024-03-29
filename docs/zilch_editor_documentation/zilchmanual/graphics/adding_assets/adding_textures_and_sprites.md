[SpriteSource](../../../../code_reference/class_reference/spritesource.md) is the Resource used to create [Sprites](../sprites/sprite.md), which represent all 2D graphical assets in Zilch.  Sprites can take the form of a single 2D image or a SpriteSheet displaying all the Sprites needed for an animation in the same file. See [resourceadding](../../editor/editorcommands/resourceadding.md) for how to import an image as a SpriteSource.

NOTE: The only file format that may be imported to create a SpriteSource is `.png`. Other formats, such as `.jpg`, are lossy and can result in undesirable artifacts, especially when scaled. If the image only exists as a `.jpg` and it is absolutely necessary, there are a number of websites that offer free conversion from `.jpg` (and many other formats) to `.png`.

 #  SpriteSource Setup
To change the values applied to a SpriteSource when an image is imported, double-click the appropriate SpriteSource from the Library window window, which will open the [Sprite Source Editor](../sprites/spritesourceeditor.md):



![SpriteSourceEditor](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47311.png) *Sprite Source Editor window*


There are many different properties that may be modified such as where to set the origin, the type of sampling, and the SpriteFill mode (to change from Fill to [Nine Slice](../sprites/area.md) for example). If the SpriteSource is a sprite sheet created for [Sprite animation](../sprites/spritesourceeditor.md#creating-sprite-animatio), click on `Convert to Animation` to open the Sprite Importer window.

 # Related Material

 ## Manual
 [BaseSprite](../sprites/basesprite.md)
 [Sprite](../sprites/sprite.md)
 [Sprite Source Editor](../sprites/spritesourceeditor.md)
 [Block Compression](block_compression.md)

 ## Reference
 [SpriteSource](../../../code_reference/class_reference/spritesource.md) 
 [Sprite](../../../code_reference/class_reference/sprite.md)  

 
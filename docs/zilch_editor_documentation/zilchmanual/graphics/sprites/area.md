The [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md) Component is a very powerful tool when working with [Sprites](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/sprite.md) or [SpriteTexts](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritetext.md), allowing for the manipulation of sizes without losing visual acuity. It is able to work in conjunction with the [SpriteSourceEditor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritesourceeditor.md) in order to define the Area that the Sprite or SpriteText cover.

 # Nine-Slicing Sprites
Often when scaling Sprites (particularly UI sprites) the edges of the sprite will be stretched causing undesirable results as can be seen here:



![Stretched](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47770.png)


By adding an Area Component instead, the Sprite can be enlarged without having the issues of blurry and stretched edges. Changing the SpriteFill enum option found in the SpriteSourceEditor to `NineSlice`



![ninesliceoptions](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/1150.png)


and then changing the Left , Right , Top , and Bottom  options that come after it changes the borders the Sprite uses to Stretch. It then stretches based on this format instead:



![nineslicedemo](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/1151.png)


By using these options instead of simply using Scale , Sprites can be increased in size while still being clear visually.



![WithArea](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47772.png)


 # Tiling Sprites
Similar to using the `NineSlice` option, any Sprite can use the Area in order to tile itself and repeatedly copy itself when stretched. 



![TileNoArea](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47774.png)


Adjusting the Scale of a Sprite like this isn't the solution. Instead attach the Area Component and change the SpriteFill enum option in the SpriteSourceEditor to `Tiled`.



![tiledoptions](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/1154.png)


This will allow the Area component to properly adjust and repeat the image as Size  is increased beyond the original scale of the SpriteSource. 



![Tiled](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47776.png)


 # Organizing Text

By utilizing the Area Component alongside the [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritetext.md) componet, it becomes possible to gain a large amount of control over how the SpriteText is displayed.

Adding the Area Component will give the ability to define the area the text is displayed in, while retaining the alignment set in the SpriteText component. It also will use word wrapping to make sure no text spills outside of the defined area.



![Text](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47782.gif)


 # Related Materials
 ## Manual Pages
- [sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/sprite.md)
- [spritetext](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritetext.md)
- [spritesourceeditor](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/spritesourceeditor.md)

 ## Reference Pages
- [Area](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/area.md)
- [Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sprite.md) 
- [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md) 

 
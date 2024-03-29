A [SpriteSource](../../../code_reference/class_reference/spritesource.md) is used to create a two dimensional visual element. SpriteSources can be added and modified as needed, and the same base image can be used to create several different SpriteSources if need be. 

 # Common Uses

 - Characters and other artwork in a two dimensional project
 - Placing 2D pictures into a 3D landscape
 - 2D animations

 # Adding a SpriteSource

NOTE: **Zilch Engine only allows the importing of .PNG type images.**

It is possible to add SpriteSources of your own as well. By dragging a .png file into the Editor window, Zilch Engine will import the chosen asset. Alternatively, using the [Command](../../editor/editorcommands/commands.md) : `Add` and selecting SpriteSource from the list followed by clicking on `From File`, will open a new window. The user may then select the image or images to import into the engine, keeping the saved Resolution and Size. Once imported, these files can then be assigned to a game object with the Sprite component by clicking on the current SpriteSource and finding the imported image in the drop-down menu that opens.



![ChooseSpriteSource](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47420.gif)


If changes need to be made, the SpriteSource can be modified in the [Sprite Source Editor](../../graphics/sprites/spritesourceeditor.md). 

 # Related Materials
 ## Manual Pages
- [Sprites](../../graphics/sprites/sprite.md)
- [SpriteSource Editor](../../graphics/sprites/spritesourceeditor.md)
- [Adding a Resource](../../editor/editorcommands/resourceadding.md)

 ## Tutorials
- [Sprites](../../../tutorials/graphics/spritesandtext/sprites.md)

 ## Reference Pages
- [SpriteSource](../../../code_reference/class_reference/spritesource.md) 
 

 
(NOTE)**Recommended Reading**  This section covers topics that may not have been addressed yet. To learn or review those topics, please see: [Base Sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/basesprite.md)

[spritetext](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/spritetext.md) is a useful component for quickly adding text into a project that allows the user to easily modify the properties of the text, such as the [font](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources/font.md), size, and runtime output. As with [sprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/sprite.md), SpriteText can be added to any existing [Game Object](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/cogs/gameobjectsconcept.md). 

 # Common Uses
 - Scores, timers, and other HUD texts
 - Title, menu and button text

 # Using SpriteText
 ## Creating SpriteText
SpriteText can be made in different two ways: using the [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : CreateSpriteText  or adding the `SpriteText` Component to any existing Game Object. The actual font is defined by the Font resource property, and all other properties control how the font is displayed:  The only differences in the objects are the values of a few properties:



![SpriteTextProperties](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47818.png) *SpriteText Component*


 ## Adding new Fonts
Importing and accessing different Font resource resources is arguably the most important thing to understand regarding SpriteText. Luckily, Zilch Engine makes this very simple, allowing the user to drag and drop the [font](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources/font.md) into the Editor window. Alternatively, the user can use either [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands/commands.md) : Add  or click on the Add button button and select `Font  > IMPORT FONT`:



![AddButton](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47820.png) *Resource Add Button*




![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/45994.png) *Adding a Font*


This will open a new file explorer window where the user may select the Font or Fonts to import. Once a Font is imported into Zilch, simply select the Font resource property on the SpriteText component and choose the desired Font.



![ChangeFonts](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47827.gif) *Selecting Multiple Fonts*


NOTE: Zilch accepts both OpenType Font (OTF) and TrueType Font (TTF).


 ## Changing the Text
Typing the desired text into the Text  property and changing the FontSize  will adjust the text on screen, but that's also a bare minimum of what SpriteText is able to do. For example, by adjusting the PixelsPerUnit  property, it becomes possible to create different sized Fonts without losing any visual clarity.

 # Related Materials
 ## Manual Pages
- [BaseSprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/graphics/sprites/basesprite.md)
- [TextBlock](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources/textblock.md)

 ## Reference Pages
- [SpriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/spritetext.md)
- [Font](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/font.md)
- [Camera](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/camera.md)
- [Event](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/code_reference/class_reference/event.md) 

 
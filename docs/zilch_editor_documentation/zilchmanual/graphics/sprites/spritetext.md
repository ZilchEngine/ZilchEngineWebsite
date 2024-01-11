(NOTE)**Recommended Reading**  This section covers topics that may not have been addressed yet. To learn or review those topics, please see: [Base Sprite](basesprite.md)

[spritetext](../../../code_reference/class_reference/spritetext.md) is a useful component for quickly adding text into a project that allows the user to easily modify the properties of the text, such as the [font](../../architecture/resources/font.md), size, and runtime output. As with [sprite](../../../code_reference/class_reference/sprite.md), SpriteText can be added to any existing [Game Object](../../architecture/cogs/gameobjectsconcept.md). 

 # Common Uses
 - Scores, timers, and other HUD texts
 - Title, menu and button text

 # Using SpriteText
 ## Creating SpriteText
SpriteText can be made in different two ways: using the [Command](../../editor/editorcommands/commands.md) : CreateSpriteText  or adding the `SpriteText` Component to any existing Game Object. The actual font is defined by the Font resource property, and all other properties control how the font is displayed:  The only differences in the objects are the values of a few properties:



![SpriteTextProperties](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47818.png) *SpriteText Component*


 ## Adding new Fonts
Importing and accessing different Font resource resources is arguably the most important thing to understand regarding SpriteText. Luckily, Zilch Engine makes this very simple, allowing the user to drag and drop the [font](../../architecture/resources/font.md) into the Editor window. Alternatively, the user can use either [Command](../../editor/editorcommands/commands.md) : Add  or click on the Add button button and select `Font  > IMPORT FONT`:



![AddButton](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47820.png) *Resource Add Button*




![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/45994.png) *Adding a Font*


This will open a new file explorer window where the user may select the Font or Fonts to import. Once a Font is imported into Zilch, simply select the Font resource property on the SpriteText component and choose the desired Font.



![ChangeFonts](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47827.gif) *Selecting Multiple Fonts*


NOTE: Zilch accepts both OpenType Font (OTF) and TrueType Font (TTF).


 ## Changing the Text
Typing the desired text into the Text  property and changing the FontSize  will adjust the text on screen, but that's also a bare minimum of what SpriteText is able to do. For example, by adjusting the PixelsPerUnit  property, it becomes possible to create different sized Fonts without losing any visual clarity.

 # Related Materials
 ## Manual Pages
- [BaseSprite](basesprite.md)
- [TextBlock](../../architecture/resources/textblock.md)

 ## Reference Pages
- [SpriteText](../../../code_reference/class_reference/spritetext.md)
- [Font](../../../code_reference/class_reference/font.md)
- [Camera](../../../code_reference/class_reference/camera.md)
- [Event](../../../code_reference/class_reference/event.md) 

 
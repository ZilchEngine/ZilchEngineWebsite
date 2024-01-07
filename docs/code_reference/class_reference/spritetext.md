 `Component` `Graphics`



(NOTE) Text that is rendered from a texture atlas in the same way that Sprites are.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCharacterPosition](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#getcharacterposition-zer)|[ Font](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#font-zilch-engine-documen)|[basesprite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/basesprite.md)| |
|[ MeasureGivenText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#measuregiventext-zilch-en)|[ FontSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#fontsize-zilch-engine-doc)| | |
|[ MeasureText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#measuretext-zilch-engine)|[ PixelsPerUnit](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#pixelsperunit-zilch-engin)| | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#spritetext-void)|[ Text](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#text-zilch-engine-documen)| | |
| |[ TextAlign](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/spritetext.md#textalign-zilch-engine-do)| | |


 #  Properties


---  
 #  Font : [font](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/font.md)

> Font used to display the text.
> ``` lang=cpp, name=Nada
> var Font : Font


---  
 #  FontSize : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Size that the font will be rastered at to a texture atlas.
> ``` lang=cpp, name=Nada
> var FontSize : Integer


---  
 #  PixelsPerUnit : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Number of pixels of the font size that map to one world space unit.
> ``` lang=cpp, name=Nada
> var PixelsPerUnit : Real


---  
 #  Text : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Text to display.
> ``` lang=cpp, name=Nada
> var Text : String


---  
 #  TextAlign : [TextAlign](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#textalign)

> How to position the text about the objects origin.
> ``` lang=cpp, name=Nada
> var TextAlign : TextAlign


---  
 #  Methods


---  
 #  GetCharacterPosition : [real3](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real3.md)

> Get the position in world space of a character by index.
> |Name|Type|Description|
> |---|---|---|
> |characterIndex|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function GetCharacterPosition(characterIndex : Integer) : Real3
> ``` 


---  
 #  MeasureGivenText : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Get the effective size in world space that the SpriteText would be if this was its text.
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function MeasureGivenText(text : String) : Real2
> ``` 


---  
 #  MeasureText : [real2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real2.md)

> Get the effective size in world space of the current text.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MeasureText() : Real2
> ``` 


---  
 #  SpriteText : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function SpriteText()
> ``` 


---  
 

 
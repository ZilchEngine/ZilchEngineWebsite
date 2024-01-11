 `Component` `Graphics`



(NOTE) Text that is rendered from a texture atlas in the same way that Sprites are.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetCharacterPosition](spritetext.md#getcharacterposition-zer)|[ Font](spritetext.md#font-zilch-engine-documen)|[basesprite](basesprite.md)| |
|[ MeasureGivenText](spritetext.md#measuregiventext-zilch-en)|[ FontSize](spritetext.md#fontsize-zilch-engine-doc)| | |
|[ MeasureText](spritetext.md#measuretext-zilch-engine)|[ PixelsPerUnit](spritetext.md#pixelsperunit-zilch-engin)| | |
|[ Constructor](spritetext.md#spritetext-void)|[ Text](spritetext.md#text-zilch-engine-documen)| | |
| |[ TextAlign](spritetext.md#textalign-zilch-engine-do)| | |


 #  Properties


---  
 #  Font : [font](font.md)

> Font used to display the text.
> ```TS:Nada
> var Font : Font


---  
 #  FontSize : [integer](../nada_base_types/integer.md)

> Size that the font will be rastered at to a texture atlas.
> ```TS:Nada
> var FontSize : Integer


---  
 #  PixelsPerUnit : [real](../nada_base_types/real.md)

> Number of pixels of the font size that map to one world space unit.
> ```TS:Nada
> var PixelsPerUnit : Real


---  
 #  Text : [string](../nada_base_types/string.md)

> Text to display.
> ```TS:Nada
> var Text : String


---  
 #  TextAlign : [TextAlign](../enum_reference.md#textalign)

> How to position the text about the objects origin.
> ```TS:Nada
> var TextAlign : TextAlign


---  
 #  Methods


---  
 #  GetCharacterPosition : [real3](../nada_base_types/real3.md)

> Get the position in world space of a character by index.
> |Name|Type|Description|
> |---|---|---|
> |characterIndex|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetCharacterPosition(characterIndex : Integer) : Real3
> ``` 


---  
 #  MeasureGivenText : [real2](../nada_base_types/real2.md)

> Get the effective size in world space that the SpriteText would be if this was its text.
> |Name|Type|Description|
> |---|---|---|
> |text|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function MeasureGivenText(text : String) : Real2
> ``` 


---  
 #  MeasureText : [real2](../nada_base_types/real2.md)

> Get the effective size in world space of the current text.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function MeasureText() : Real2
> ``` 


---  
 #  SpriteText : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function SpriteText()
> ``` 


---  
 

 
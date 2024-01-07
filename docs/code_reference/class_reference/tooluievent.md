 `Event` `Editor`



(NOTE) Allows Ui customization for Tools. This will be sent on the Tool every time it is activated.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[ NeedsPropertyGrid](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tooluievent.md#needspropertygrid-zilch-e)|[event](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/event.md)| |
| |[ Parent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tooluievent.md#parent-zilch-engine-docum)| | |
| |[ SelectTool](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tooluievent.md#selecttool-zilch-engine-d)| | |


 #  Properties


---  
 #  NeedsPropertyGrid : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Whether or not to force show the tools window when switched to this tool.
> ``` lang=cpp, name=Nada
> var NeedsPropertyGrid : Boolean


---  
 #  Parent : [composite](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/composite.md)

 `read-only`

> Getters / setters.
> ``` lang=cpp, name=Nada
> var Parent : Composite


---  
 #  SelectTool : [cog](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/cog.md)

 `read-only`

> Easy access to the Select Tool. It's commonly used in other Tools (such as ray casting).
> ``` lang=cpp, name=Nada
> var SelectTool : Cog


---  
 #  Methods


---  
 

 
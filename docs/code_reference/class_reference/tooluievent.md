 `Event` `Editor`



(NOTE) Allows Ui customization for Tools. This will be sent on the Tool every time it is activated.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
| |[NeedsPropertyGrid](tooluievent.md#needspropertygrid-zilch-e)|[event](event.md)| |
| |[Parent](tooluievent.md#parent-zilch-engine-docum)| | |
| |[SelectTool](tooluievent.md#selecttool-zilch-engine-d)| | |


 #  Properties


---  
 #  NeedsPropertyGrid : [boolean](../nada_base_types/boolean.md)

> Whether or not to force show the tools window when switched to this tool.
> ```TS:Nada
> var NeedsPropertyGrid : Boolean


---  
 #  Parent : [composite](composite.md)

 `read-only`

> Getters / setters.
> ```TS:Nada
> var Parent : Composite


---  
 #  SelectTool : [cog](cog.md)

 `read-only`

> Easy access to the Select Tool. It's commonly used in other Tools (such as ray casting).
> ```TS:Nada
> var SelectTool : Cog


---  
 #  Methods


---  
 

 
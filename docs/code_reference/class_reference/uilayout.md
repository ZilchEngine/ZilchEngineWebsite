 `Component` `UiWidget`



(NOTE) Layouts are in charge of calling UpdateTransform on all children, regardless of whether or not they ignore layouts.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Debug](uilayout.md#debug-void)|[ PaddingBottom](uilayout.md#paddingbottom-zilch-engin)|[component](component.md)|[uidocklayout](uidocklayout.md)|
| |[ PaddingLeft](uilayout.md#paddingleft-zilch-engine)| |[uifilllayout](uifilllayout.md)|
| |[ PaddingRight](uilayout.md#paddingright-zilch-engine)| |[uistacklayout](uistacklayout.md)|
| |[ PaddingTop](uilayout.md#paddingtop-zilch-engine-d)| | |


 #  Properties


---  
 #  PaddingBottom : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var PaddingBottom : Real


---  
 #  PaddingLeft : [real](../nada_base_types/real.md)

> Padding getter / setters for binding until we have Thickness binding.
> ```TS:Nada
> var PaddingLeft : Real


---  
 #  PaddingRight : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var PaddingRight : Real


---  
 #  PaddingTop : [real](../nada_base_types/real.md)

> 
> ```TS:Nada
> var PaddingTop : Real


---  
 #  Methods


---  
 #  Debug : Void

> Calling this will set a breakpoint before the layout is done.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Debug()
> ``` 


---  
 

 
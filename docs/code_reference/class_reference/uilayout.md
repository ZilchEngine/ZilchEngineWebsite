 `Component` `UiWidget`



(NOTE) Layouts are in charge of calling UpdateTransform on all children, regardless of whether or not they ignore layouts.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Debug](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilayout.md#debug-void)|[ PaddingBottom](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilayout.md#paddingbottom-zilch-engin)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)|[uidocklayout](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uidocklayout.md)|
| |[ PaddingLeft](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilayout.md#paddingleft-zilch-engine)| |[uifilllayout](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uifilllayout.md)|
| |[ PaddingRight](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilayout.md#paddingright-zilch-engine)| |[uistacklayout](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uistacklayout.md)|
| |[ PaddingTop](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/uilayout.md#paddingtop-zilch-engine-d)| | |


 #  Properties


---  
 #  PaddingBottom : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var PaddingBottom : Real


---  
 #  PaddingLeft : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> Padding getter / setters for binding until we have Thickness binding.
> ``` lang=cpp, name=Nada
> var PaddingLeft : Real


---  
 #  PaddingRight : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var PaddingRight : Real


---  
 #  PaddingTop : [real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)

> 
> ``` lang=cpp, name=Nada
> var PaddingTop : Real


---  
 #  Methods


---  
 #  Debug : Void

> Calling this will set a breakpoint before the layout is done.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Debug()
> ``` 


---  
 

 
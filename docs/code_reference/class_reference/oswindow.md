 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClientToScreen](oswindow.md#clienttoscreen-zilch-engi)|[ ClientSize](oswindow.md#clientsize-zilch-engine-d)|[threadsafeid32eventobject](threadsafeid32eventobject.md)|[windowsoswindow](windowsoswindow.md)|
|[ HasFocus](oswindow.md#hasfocus-zilch-engine-doc)|[ MinSize](oswindow.md#minsize-zilch-engine-docu)| | |
|[ ScreenToClient](oswindow.md#screentoclient-zilch-engi)|[ MouseCapture](oswindow.md#mousecapture-zilch-engine)| | |
| |[ MouseCursor](oswindow.md#mousecursor-zilch-engine)| | |
| |[ MouseTrap](oswindow.md#mousetrap-zilch-engine-do)| | |
| |[ Parent](oswindow.md#parent-zilch-engine-docum)| | |
| |[ Position](oswindow.md#position-zilch-engine-doc)| | |
| |[ Size](oswindow.md#size-zilch-engine-documen)| | |
| |[ State](oswindow.md#state-zilch-engine-docume)| | |
| |[ Title](oswindow.md#title-zilch-engine-docume)| | |
| |[ Visible](oswindow.md#visible-zilch-engine-docu)| | |


 #  Properties


---  
 #  ClientSize : [integer2](../nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var ClientSize : Integer2


---  
 #  MinSize : [integer2](../nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var MinSize : Integer2


---  
 #  MouseCapture : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var MouseCapture : Boolean


---  
 #  MouseCursor : [Cursor](../enum_reference.md#cursor)

> 
> ``` lang=cpp, name=Nada
> var MouseCursor : Cursor


---  
 #  MouseTrap : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var MouseTrap : Boolean


---  
 #  Parent : [oswindow](oswindow.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Parent : OsWindow


---  
 #  Position : [integer2](../nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var Position : Integer2


---  
 #  Size : [integer2](../nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var Size : Integer2


---  
 #  State : [WindowState](../enum_reference.md#windowstate)

> 
> ``` lang=cpp, name=Nada
> var State : WindowState


---  
 #  Title : [string](../nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Title : String


---  
 #  Visible : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Visible : Boolean


---  
 #  Methods


---  
 #  ClientToScreen : [integer2](../nada_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function ClientToScreen(p0 : Integer2) : Integer2
> ``` 


---  
 #  HasFocus : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function HasFocus() : Boolean
> ``` 


---  
 #  ScreenToClient : [integer2](../nada_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function ScreenToClient(p0 : Integer2) : Integer2
> ``` 


---  
 

 
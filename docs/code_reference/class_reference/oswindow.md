 `Engine`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ ClientToScreen](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#clienttoscreen-zilch-engi)|[ ClientSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#clientsize-zilch-engine-d)|[threadsafeid32eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/threadsafeid32eventobject.md)|[windowsoswindow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/windowsoswindow.md)|
|[ HasFocus](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#hasfocus-zilch-engine-doc)|[ MinSize](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#minsize-zilch-engine-docu)| | |
|[ ScreenToClient](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#screentoclient-zilch-engi)|[ MouseCapture](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#mousecapture-zilch-engine)| | |
| |[ MouseCursor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#mousecursor-zilch-engine)| | |
| |[ MouseTrap](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#mousetrap-zilch-engine-do)| | |
| |[ Parent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#parent-zilch-engine-docum)| | |
| |[ Position](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#position-zilch-engine-doc)| | |
| |[ Size](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#size-zilch-engine-documen)| | |
| |[ State](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#state-zilch-engine-docume)| | |
| |[ Title](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#title-zilch-engine-docume)| | |
| |[ Visible](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md#visible-zilch-engine-docu)| | |


 #  Properties


---  
 #  ClientSize : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var ClientSize : Integer2


---  
 #  MinSize : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var MinSize : Integer2


---  
 #  MouseCapture : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var MouseCapture : Boolean


---  
 #  MouseCursor : [Cursor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#cursor)

> 
> ``` lang=cpp, name=Nada
> var MouseCursor : Cursor


---  
 #  MouseTrap : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var MouseTrap : Boolean


---  
 #  Parent : [oswindow](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/oswindow.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Parent : OsWindow


---  
 #  Position : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var Position : Integer2


---  
 #  Size : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var Size : Integer2


---  
 #  State : [WindowState](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#windowstate)

> 
> ``` lang=cpp, name=Nada
> var State : WindowState


---  
 #  Title : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Title : String


---  
 #  Visible : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Visible : Boolean


---  
 #  Methods


---  
 #  ClientToScreen : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function ClientToScreen(p0 : Integer2) : Integer2
> ``` 


---  
 #  HasFocus : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function HasFocus() : Boolean
> ``` 


---  
 #  ScreenToClient : [integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function ScreenToClient(p0 : Integer2) : Integer2
> ``` 


---  
 

 
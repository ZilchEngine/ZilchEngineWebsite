 `Gameplay`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Create](webbrowser.md#create-zilch-engine-docum)|[ BackgroundColor](webbrowser.md#backgroundcolor-zilch-eng)|[referencecountedeventobject](referencecountedeventobject.md)| |
|[ ExecuteScript](webbrowser.md#executescript-void)|[ CanGoBackward](webbrowser.md#cangobackward-zilch-engin)| | |
|[ ExecuteScriptFromLocation](webbrowser.md#executescriptfromlocatio)|[ CanGoForward](webbrowser.md#cangoforward-zilch-engine)| | |
|[ GoBackward](webbrowser.md#gobackward-void)|[ Focus](webbrowser.md#focus-zilch-engine-docume)| | |
|[ GoForward](webbrowser.md#goforward-void)|[ IsLoading](webbrowser.md#isloading-zilch-engine-do)| | |
|[ Reload](webbrowser.md#reload-void)|[ ScrollSpeed](webbrowser.md#scrollspeed-zilch-engine)| | |
|[ SimulateKey](webbrowser.md#simulatekey-void)|[ Size](webbrowser.md#size-zilch-engine-documen)| | |
|[ SimulateMouseClick](webbrowser.md#simulatemouseclick-void)|[ Status](webbrowser.md#status-zilch-engine-docum)| | |
|[ SimulateMouseDoubleClick](webbrowser.md#simulatemousedoubleclick)|[ Texture](webbrowser.md#texture-zilch-engine-docu)| | |
|[ SimulateMouseMove](webbrowser.md#simulatemousemove-void)|[ Title](webbrowser.md#title-zilch-engine-docume)| | |
|[ SimulateMouseScroll](webbrowser.md#simulatemousescroll-void)|[ Transparent](webbrowser.md#transparent-zilch-engine)| | |
|[ SimulateTextTyped](webbrowser.md#simulatetexttyped-void)|[ Url](webbrowser.md#url-zilch-engine-document)| | |
| |[ Visible](webbrowser.md#visible-zilch-engine-docu)| | |


 #  Properties


---  
 #  BackgroundColor : [real4](../nada_base_types/real4.md)

> 
> ``` lang=cpp, name=Nada
> var BackgroundColor : Real4


---  
 #  CanGoBackward : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CanGoBackward : Boolean


---  
 #  CanGoForward : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var CanGoForward : Boolean


---  
 #  Focus : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Focus : Boolean


---  
 #  IsLoading : [boolean](../nada_base_types/boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsLoading : Boolean


---  
 #  ScrollSpeed : [real2](../nada_base_types/real2.md)

> 
> ``` lang=cpp, name=Nada
> var ScrollSpeed : Real2


---  
 #  Size : [integer2](../nada_base_types/integer2.md)

> 
> ``` lang=cpp, name=Nada
> var Size : Integer2


---  
 #  Status : [string](../nada_base_types/string.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Status : String


---  
 #  Texture : [texture](texture.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Texture : Texture


---  
 #  Title : [string](../nada_base_types/string.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Title : String


---  
 #  Transparent : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Transparent : Boolean


---  
 #  Url : [string](../nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Url : String


---  
 #  Visible : [boolean](../nada_base_types/boolean.md)

> 
> ``` lang=cpp, name=Nada
> var Visible : Boolean


---  
 #  Methods


---  
 #  Create : [webbrowser](webbrowser.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Create() : WebBrowser
> ``` 


---  
 #  Create : [webbrowser](webbrowser.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[webbrowsersetup](webbrowsersetup.md)| |
> ``` lang=cpp, name=Nada
> function Create(p0 : WebBrowserSetup) : WebBrowser
> ``` 


---  
 #  ExecuteScript : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function ExecuteScript(p0 : String)
> ``` 


---  
 #  ExecuteScriptFromLocation : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](../nada_base_types/string.md)| |
> |p1|[string](../nada_base_types/string.md)| |
> |p2|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function ExecuteScriptFromLocation(p0 : String, p1 : String, p2 : Integer)
> ``` 


---  
 #  GoBackward : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GoBackward()
> ``` 


---  
 #  GoForward : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function GoForward()
> ``` 


---  
 #  Reload : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Reload()
> ``` 


---  
 #  Reload : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Reload(p0 : Boolean)
> ``` 


---  
 #  SimulateKey : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](../nada_base_types/integer.md)| |
> |p1|[boolean](../nada_base_types/boolean.md)| |
> |p2|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateKey(p0 : Integer, p1 : Boolean, p2 : WebBrowserModifiers)
> ``` 


---  
 #  SimulateMouseClick : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> |p1|[MouseButtons](../enum_reference.md#mousebuttons)| |
> |p2|[boolean](../nada_base_types/boolean.md)| |
> |p3|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateMouseClick(p0 : Integer2, p1 : MouseButtons, p2 : Boolean, p3 : WebBrowserModifiers)
> ``` 


---  
 #  SimulateMouseDoubleClick : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> |p1|[MouseButtons](../enum_reference.md#mousebuttons)| |
> |p2|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateMouseDoubleClick(p0 : Integer2, p1 : MouseButtons, p2 : WebBrowserModifiers)
> ``` 


---  
 #  SimulateMouseMove : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> |p1|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateMouseMove(p0 : Integer2, p1 : WebBrowserModifiers)
> ``` 


---  
 #  SimulateMouseScroll : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer2](../nada_base_types/integer2.md)| |
> |p1|[real2](../nada_base_types/real2.md)| |
> |p2|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateMouseScroll(p0 : Integer2, p1 : Real2, p2 : WebBrowserModifiers)
> ``` 


---  
 #  SimulateTextTyped : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](../nada_base_types/integer.md)| |
> |p1|[WebBrowserModifiers](../enum_reference.md#webbrowsermodifiers)| |
> ``` lang=cpp, name=Nada
> function SimulateTextTyped(p0 : Integer, p1 : WebBrowserModifiers)
> ``` 


---  
 

 
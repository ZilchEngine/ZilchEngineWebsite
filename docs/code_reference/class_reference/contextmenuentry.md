 `Widget`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ AddCommandByName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#addcommandbyname-zilch-en)|[ Icon](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#icon-zilch-engine-documen)|[safeid32eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/safeid32eventobject.md)|[contextmenuentrycommand](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentrycommand.md)|
|[ AddDivider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#adddivider-zilch-engine-d)|[ Name](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#name-zilch-engine-documen)| |[contextmenuentrydivider](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentrydivider.md)|
|[ AddEntry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#addentry-zilch-engine-doc)| | |[contextmenuentrymenu](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentrymenu.md)|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#contextmenuentry-void)| | | |
|[ Entries](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#entries-zilch-engine-docu)| | | |
|[ GetEntry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#getentry-zilch-engine-doc)| | | |
|[ RemoveEntry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md#removeentry-void)| | | |


 #  Properties


---  
 #  Icon : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Icon : String


---  
 #  Name : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> ``` lang=cpp, name=Nada
> var Name : String


---  
 #  Methods


---  
 #  AddCommandByName : [contextmenuentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |commandName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function AddCommandByName(commandName : String) : ContextMenuEntry
> ``` 


---  
 #  AddDivider : [contextmenuentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function AddDivider() : ContextMenuEntry
> ``` 


---  
 #  AddEntry : [contextmenuentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md)

> Adds a new entry with the provided name with an icon if one is provided to this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function AddEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  ContextMenuEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ContextMenuEntry()
> ``` 


---  
 #  Entries : [contextmenuentrychildrenrange](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentrychildrenrange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Entries() : ContextMenuEntryChildrenRange
> ``` 


---  
 #  GetEntry : [contextmenuentry](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/contextmenuentry.md)

> Returns the children entry with the provided name if it exists and null otherwise.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function GetEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  RemoveEntry : Void

> Remove the entry with the provided name from this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function RemoveEntry(name : String)
> ``` 


---  
 

 
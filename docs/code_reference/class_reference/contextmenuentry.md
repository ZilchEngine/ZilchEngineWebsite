 `Widget`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddCommandByName](contextmenuentry.md#addcommandbyname-zilch-en)|[Icon](contextmenuentry.md#icon-zilch-engine-documen)|[safeid32eventobject](safeid32eventobject.md)|[contextmenuentrycommand](contextmenuentrycommand.md)|
|[AddDivider](contextmenuentry.md#adddivider-zilch-engine-d)|[Name](contextmenuentry.md#name-zilch-engine-documen)| |[contextmenuentrydivider](contextmenuentrydivider.md)|
|[AddEntry](contextmenuentry.md#addentry-zilch-engine-doc)| | |[contextmenuentrymenu](contextmenuentrymenu.md)|
|[Constructor](contextmenuentry.md#contextmenuentry-void)| | | |
|[Entries](contextmenuentry.md#entries-zilch-engine-docu)| | | |
|[GetEntry](contextmenuentry.md#getentry-zilch-engine-doc)| | | |
|[RemoveEntry](contextmenuentry.md#removeentry-void)| | | |


 #  Properties


---  
 #  Icon : [string](../nada_base_types/string.md)

> 
> ```TS:Nada
> var Icon : String


---  
 #  Name : [string](../nada_base_types/string.md)

> 
> ```TS:Nada
> var Name : String


---  
 #  Methods


---  
 #  AddCommandByName : [contextmenuentry](contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |commandName|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function AddCommandByName(commandName : String) : ContextMenuEntry
> ``` 


---  
 #  AddDivider : [contextmenuentry](contextmenuentry.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AddDivider() : ContextMenuEntry
> ``` 


---  
 #  AddEntry : [contextmenuentry](contextmenuentry.md)

> Adds a new entry with the provided name with an icon if one is provided to this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function AddEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  ContextMenuEntry : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ContextMenuEntry()
> ``` 


---  
 #  Entries : [contextmenuentrychildrenrange](contextmenuentrychildrenrange.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Entries() : ContextMenuEntryChildrenRange
> ``` 


---  
 #  GetEntry : [contextmenuentry](contextmenuentry.md)

> Returns the children entry with the provided name if it exists and null otherwise.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function GetEntry(name : String) : ContextMenuEntry
> ``` 


---  
 #  RemoveEntry : Void

> Remove the entry with the provided name from this menu entries children.
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function RemoveEntry(name : String)
> ``` 


---  
 

 
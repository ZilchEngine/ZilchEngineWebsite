 `Engine`

(NOTE) Keyboard representing the physical keyboard.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ GetKeyName](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#getkeyname-zilch-engine-d)| |[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ IsAnyKeyDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#isanykeydown-zilch-engine)| | | |
|[ IsAnyNonModifierDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#isanynonmodifierdown-zer)| | | |
|[ KeyIsDown](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisdown-zilch-engine-do)| | | |
|[ KeyIsPressed](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyispressed-zilch-engine)| | | |
|[ KeyIsReleased](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisreleased-zilch-engin)| | | |
|[ KeyIsUp](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#keyisup-zilch-engine-docu)| | | |
|[ ToKey](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#tokey-zilch-engine-docume)| | | |
|[ ToSymbol](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#tosymbol-zilch-engine-doc)| | | |
|[ Valid](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/keyboard.md#valid-zilch-engine-docume)| | | |


 #  Properties


---  
 #  Methods


---  
 #  GetKeyName : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Gets a string name of a particular key.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function GetKeyName(key : Keys) : String
> ``` 


---  
 #  IsAnyKeyDown : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsAnyKeyDown() : Boolean
> ``` 


---  
 #  IsAnyNonModifierDown : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Excluding Ctrl, Shift, and Alt - is any key in the 'Keys' enum down (not including 'Keys::Unknown', e.g. PrintScreen).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsAnyNonModifierDown() : Boolean
> ``` 


---  
 #  KeyIsDown : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the particular currently down.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function KeyIsDown(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsPressed : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Was the key pressed this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function KeyIsPressed(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsReleased : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Was the key released this frame.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function KeyIsReleased(key : Keys) : Boolean
> ``` 


---  
 #  KeyIsUp : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Is the particular currently up.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function KeyIsUp(key : Keys) : Boolean
> ``` 


---  
 #  ToKey : [Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)

> Counterpart to 'ToSymbol'. Converts a key's name or symbol to the key value. Returns Keys::Unknown if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function ToKey(key : String) : Keys
> ``` 


---  
 #  ToSymbol : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Convert key value to it's actual name or keyboard symbol, if it has one. Returns "Unknown" String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function ToSymbol(key : Keys) : String
> ``` 


---  
 #  ToSymbol : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Convert a key name to it's keyboard symbol, if it has one. Returns input String if key is not found.
> |Name|Type|Description|
> |---|---|---|
> |keyName|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function ToSymbol(keyName : String) : String
> ``` 


---  
 #  Valid : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Validate that the key is a Keys::Enum that is not 'Unknown', or 'None', or an integer value that doesn't map to a known Keys::Enum value.
> |Name|Type|Description|
> |---|---|---|
> |key|[Keys](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#keys)| |
> ``` lang=cpp, name=Nada
> function Valid(key : Keys) : Boolean
> ``` 


---  
 #  Valid : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Validate that the input string can be mapped back to an enum.
> |Name|Type|Description|
> |---|---|---|
> |key|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Valid(key : String) : Boolean
> ``` 


---  
 

 
 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md#iencoding-void)|[ Ascii](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md#ascii-zilch-engine-docume)| |[asciiencoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/asciiencoding.md)|
|[ Read](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md#read-zilch-engine-documen)|[ Utf8](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md#utf8-zilch-engine-documen)| |[utf8encoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/utf8encoding.md)|
|[ Write](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md#write-zilch-engine-docume)| | | |


 #  Properties


---  
 #  Ascii : [asciiencoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/asciiencoding.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Ascii : AsciiEncoding


---  
 #  Utf8 : [utf8encoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/utf8encoding.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Utf8 : Utf8Encoding


---  
 #  Methods


---  
 #  IEncoding : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IEncoding()
> ``` 


---  
 #  Read : [rune](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/rune.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[istream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md)| |
> ``` lang=cpp, name=Nada
> function Read(p0 : IStream) : Rune
> ``` 


---  
 #  Write : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/rune.md)| |
> |p1|[istream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md)| |
> ``` lang=cpp, name=Nada
> function Write(p0 : Rune, p1 : IStream) : Integer
> ``` 


---  
 

 
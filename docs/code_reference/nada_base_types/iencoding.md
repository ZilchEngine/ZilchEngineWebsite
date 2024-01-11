 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Constructor](iencoding.md#iencoding-void)|[ Ascii](iencoding.md#ascii-zilch-engine-docume)| |[asciiencoding](asciiencoding.md)|
|[ Read](iencoding.md#read-zilch-engine-documen)|[ Utf8](iencoding.md#utf8-zilch-engine-documen)| |[utf8encoding](utf8encoding.md)|
|[ Write](iencoding.md#write-zilch-engine-docume)| | | |


 #  Properties


---  
 #  Ascii : [asciiencoding](asciiencoding.md)

 `read-only` `static`

> 
> ``` lang=cpp, name=Nada
> var Ascii : AsciiEncoding


---  
 #  Utf8 : [utf8encoding](utf8encoding.md)

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
 #  Read : [rune](rune.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[istream](istream.md)| |
> ``` lang=cpp, name=Nada
> function Read(p0 : IStream) : Rune
> ``` 


---  
 #  Write : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](rune.md)| |
> |p1|[istream](istream.md)| |
> ``` lang=cpp, name=Nada
> function Write(p0 : Rune, p1 : IStream) : Integer
> ``` 


---  
 

 
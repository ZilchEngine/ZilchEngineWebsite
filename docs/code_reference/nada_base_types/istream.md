 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Flush](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#flush-void)|[ Capabilities](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#capabilities-zilch-engine)| |[filestream](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/filestream.md)|
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#istream-void)|[ Count](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#count-zilch-engine-docume)| | |
|[ Read](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#read-zilch-engine-documen)|[ Position](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#position-zilch-engine-doc)| | |
|[ ReadAllText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#readalltext-zilch-engine)| | | |
|[ ReadByte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#readbyte-zilch-engine-doc)| | | |
|[ ReadLine](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#readline-zilch-engine-doc)| | | |
|[ Seek](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#seek-zilch-engine-documen)| | | |
|[ Write](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#write-zilch-engine-docume)| | | |
|[ WriteByte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#writebyte-zilch-engine-do)| | | |
|[ WriteText](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/istream.md#writetext-zilch-engine-do)| | | |


 #  Properties


---  
 #  Capabilities : [StreamCapabilities](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/flags_reference.md#streamcapabilities)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Capabilities : StreamCapabilities


---  
 #  Count : [doubleinteger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doubleinteger.md)

> 
> ``` lang=cpp, name=Nada
> var Count : DoubleInteger


---  
 #  Position : [doubleinteger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doubleinteger.md)

> 
> ``` lang=cpp, name=Nada
> var Position : DoubleInteger


---  
 #  Methods


---  
 #  Flush : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Flush()
> ``` 


---  
 #  IStream : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IStream()
> ``` 


---  
 #  Read : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)]| |
> |byteStart|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |byteCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Read(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  ReadAllText : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadAllText() : String
> ``` 


---  
 #  ReadAllText : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md)| |
> ``` lang=cpp, name=Nada
> function ReadAllText(p0 : IEncoding) : String
> ``` 


---  
 #  ReadByte : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadByte() : Integer
> ``` 


---  
 #  ReadLine : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadLine() : String
> ``` 


---  
 #  ReadLine : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md)| |
> ``` lang=cpp, name=Nada
> function ReadLine(p0 : IEncoding) : String
> ``` 


---  
 #  Seek : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[doubleinteger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/doubleinteger.md)| |
> |origin|[StreamOrigin](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#streamorigin)| |
> ``` lang=cpp, name=Nada
> function Seek(position : DoubleInteger, origin : StreamOrigin) : Boolean
> ``` 


---  
 #  Write : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)]| |
> ``` lang=cpp, name=Nada
> function Write(data : Array[Byte]) : Integer
> ``` 


---  
 #  Write : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)]| |
> |byteStart|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |byteCount|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Write(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  WriteByte : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[byte](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/byte.md)| |
> ``` lang=cpp, name=Nada
> function WriteByte(p0 : Byte) : Integer
> ``` 


---  
 #  WriteText : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function WriteText(text : String) : Integer
> ``` 


---  
 #  WriteText : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |sourceStreamEncoding|[iencoding](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/iencoding.md)| |
> ``` lang=cpp, name=Nada
> function WriteText(text : String, sourceStreamEncoding : IEncoding) : Integer
> ``` 


---  
 

 
 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Flush](istream.md#flush-void)|[ Capabilities](istream.md#capabilities-zilch-engine)| |[filestream](filestream.md)|
|[ Constructor](istream.md#istream-void)|[ Count](istream.md#count-zilch-engine-docume)| | |
|[ Read](istream.md#read-zilch-engine-documen)|[ Position](istream.md#position-zilch-engine-doc)| | |
|[ ReadAllText](istream.md#readalltext-zilch-engine)| | | |
|[ ReadByte](istream.md#readbyte-zilch-engine-doc)| | | |
|[ ReadLine](istream.md#readline-zilch-engine-doc)| | | |
|[ Seek](istream.md#seek-zilch-engine-documen)| | | |
|[ Write](istream.md#write-zilch-engine-docume)| | | |
|[ WriteByte](istream.md#writebyte-zilch-engine-do)| | | |
|[ WriteText](istream.md#writetext-zilch-engine-do)| | | |


 #  Properties


---  
 #  Capabilities : [StreamCapabilities](../flags_reference.md#streamcapabilities)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Capabilities : StreamCapabilities


---  
 #  Count : [doubleinteger](doubleinteger.md)

> 
> ``` lang=cpp, name=Nada
> var Count : DoubleInteger


---  
 #  Position : [doubleinteger](doubleinteger.md)

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
 #  Read : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](byte.md)]| |
> |byteStart|[integer](integer.md)| |
> |byteCount|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Read(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  ReadAllText : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadAllText() : String
> ``` 


---  
 #  ReadAllText : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](iencoding.md)| |
> ``` lang=cpp, name=Nada
> function ReadAllText(p0 : IEncoding) : String
> ``` 


---  
 #  ReadByte : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadByte() : Integer
> ``` 


---  
 #  ReadLine : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ReadLine() : String
> ``` 


---  
 #  ReadLine : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](iencoding.md)| |
> ``` lang=cpp, name=Nada
> function ReadLine(p0 : IEncoding) : String
> ``` 


---  
 #  Seek : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[doubleinteger](doubleinteger.md)| |
> |origin|[StreamOrigin](../enum_reference.md#streamorigin)| |
> ``` lang=cpp, name=Nada
> function Seek(position : DoubleInteger, origin : StreamOrigin) : Boolean
> ``` 


---  
 #  Write : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](byte.md)]| |
> ``` lang=cpp, name=Nada
> function Write(data : Array[Byte]) : Integer
> ``` 


---  
 #  Write : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](byte.md)]| |
> |byteStart|[integer](integer.md)| |
> |byteCount|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function Write(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  WriteByte : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[byte](byte.md)| |
> ``` lang=cpp, name=Nada
> function WriteByte(p0 : Byte) : Integer
> ``` 


---  
 #  WriteText : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](string.md)| |
> ``` lang=cpp, name=Nada
> function WriteText(text : String) : Integer
> ``` 


---  
 #  WriteText : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](string.md)| |
> |sourceStreamEncoding|[iencoding](iencoding.md)| |
> ``` lang=cpp, name=Nada
> function WriteText(text : String, sourceStreamEncoding : IEncoding) : Integer
> ``` 


---  
 

 
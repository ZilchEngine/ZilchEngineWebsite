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
> ```TS:Nada
> var Capabilities : StreamCapabilities


---  
 #  Count : [doubleinteger](doubleinteger.md)

> 
> ```TS:Nada
> var Count : DoubleInteger


---  
 #  Position : [doubleinteger](doubleinteger.md)

> 
> ```TS:Nada
> var Position : DoubleInteger


---  
 #  Methods


---  
 #  Flush : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Flush()
> ``` 


---  
 #  IStream : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
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
> ```TS:Nada
> function Read(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  ReadAllText : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReadAllText() : String
> ``` 


---  
 #  ReadAllText : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](iencoding.md)| |
> ```TS:Nada
> function ReadAllText(p0 : IEncoding) : String
> ``` 


---  
 #  ReadByte : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReadByte() : Integer
> ``` 


---  
 #  ReadLine : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ReadLine() : String
> ``` 


---  
 #  ReadLine : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[iencoding](iencoding.md)| |
> ```TS:Nada
> function ReadLine(p0 : IEncoding) : String
> ``` 


---  
 #  Seek : [boolean](boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |position|[doubleinteger](doubleinteger.md)| |
> |origin|[StreamOrigin](../enum_reference.md#streamorigin)| |
> ```TS:Nada
> function Seek(position : DoubleInteger, origin : StreamOrigin) : Boolean
> ``` 


---  
 #  Write : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |data|Array[[byte](byte.md)]| |
> ```TS:Nada
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
> ```TS:Nada
> function Write(data : Array[Byte], byteStart : Integer, byteCount : Integer) : Integer
> ``` 


---  
 #  WriteByte : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |p0|[byte](byte.md)| |
> ```TS:Nada
> function WriteByte(p0 : Byte) : Integer
> ``` 


---  
 #  WriteText : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](string.md)| |
> ```TS:Nada
> function WriteText(text : String) : Integer
> ``` 


---  
 #  WriteText : [integer](integer.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |text|[string](string.md)| |
> |sourceStreamEncoding|[iencoding](iencoding.md)| |
> ```TS:Nada
> function WriteText(text : String, sourceStreamEncoding : IEncoding) : Integer
> ``` 


---  
 

 
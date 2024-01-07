 `Meta`

(NOTE) IPv4/IPv6 network host identifier Provided for convenience Note: This class is not slice-able, it has extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#clear-void)|[ Hash](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#hash-zilch-engine-documen)|SocketAddress| |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#ipaddress-void)|[ Host](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#host-zilch-engine-documen)| | |
| |[ InternetProtocol](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#internetprotocol-zilch-en)| | |
| |[ IsValid](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#isvalid-zilch-engine-docu)| | |
| |[ Port](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#port-zilch-engine-documen)| | |
| |[ PortString](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#portstring-zilch-engine-d)| | |
| |[ String](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md#string-zilch-engine-docum)| | |


 #  Properties


---  
 #  Hash : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Hash : Integer


---  
 #  Host : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Returns the valid IP address host as a numeric string, else String()
> ``` lang=cpp, name=Nada
> var Host : String


---  
 #  InternetProtocol : [InternetProtocol](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#internetprotocol)

 `read-only`

> Returns the valid IP address protocol version, else InternetProtocol::Unspecified.
> ``` lang=cpp, name=Nada
> var InternetProtocol : InternetProtocol


---  
 #  IsValid : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

 `read-only`

> Returns true if this is a non-empty IPv4/IPv6 address, else false.
> ``` lang=cpp, name=Nada
> var IsValid : Boolean


---  
 #  Port : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

> Returns the valid IP address port, else 0.
> ``` lang=cpp, name=Nada
> var Port : Integer


---  
 #  PortString : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Returns the valid IP address port as a numeric string, else String()
> ``` lang=cpp, name=Nada
> var PortString : String


---  
 #  String : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `read-only`

> Returns the valid IP address as a numeric "host:port" string, else String()
> ``` lang=cpp, name=Nada
> var String : String


---  
 #  Methods


---  
 #  Clear : Void

> Clears the IP address.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IpAddress()
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Copy Constructors.
> |Name|Type|Description|
> |---|---|---|
> |rhs|[ipaddress](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/ipaddress.md)| |
> ``` lang=cpp, name=Nada
> function IpAddress(rhs : IpAddress)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |port|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IpAddress(host : String, port : Integer)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |port|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |internetProtocol|[InternetProtocol](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#internetprotocol)| |
> ``` lang=cpp, name=Nada
> function IpAddress(host : String, port : Integer, internetProtocol : InternetProtocol)
> ``` 


---  
 

 
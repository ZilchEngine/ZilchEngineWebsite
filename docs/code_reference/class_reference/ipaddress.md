 `Meta`

(NOTE) IPv4/IPv6 network host identifier Provided for convenience Note: This class is not slice-able, it has extra data.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](ipaddress.md#clear-void)|[ Hash](ipaddress.md#hash-zilch-engine-documen)|SocketAddress| |
|[ Constructor](ipaddress.md#ipaddress-void)|[ Host](ipaddress.md#host-zilch-engine-documen)| | |
| |[ InternetProtocol](ipaddress.md#internetprotocol-zilch-en)| | |
| |[ IsValid](ipaddress.md#isvalid-zilch-engine-docu)| | |
| |[ Port](ipaddress.md#port-zilch-engine-documen)| | |
| |[ PortString](ipaddress.md#portstring-zilch-engine-d)| | |
| |[ String](ipaddress.md#string-zilch-engine-docum)| | |


 #  Properties


---  
 #  Hash : [integer](../nada_base_types/integer.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Hash : Integer


---  
 #  Host : [string](../nada_base_types/string.md)

> Returns the valid IP address host as a numeric string, else String()
> ``` lang=cpp, name=Nada
> var Host : String


---  
 #  InternetProtocol : [InternetProtocol](../enum_reference.md#internetprotocol)

 `read-only`

> Returns the valid IP address protocol version, else InternetProtocol::Unspecified.
> ``` lang=cpp, name=Nada
> var InternetProtocol : InternetProtocol


---  
 #  IsValid : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if this is a non-empty IPv4/IPv6 address, else false.
> ``` lang=cpp, name=Nada
> var IsValid : Boolean


---  
 #  Port : [integer](../nada_base_types/integer.md)

> Returns the valid IP address port, else 0.
> ``` lang=cpp, name=Nada
> var Port : Integer


---  
 #  PortString : [string](../nada_base_types/string.md)

 `read-only`

> Returns the valid IP address port as a numeric string, else String()
> ``` lang=cpp, name=Nada
> var PortString : String


---  
 #  String : [string](../nada_base_types/string.md)

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
> |rhs|[ipaddress](ipaddress.md)| |
> ``` lang=cpp, name=Nada
> function IpAddress(rhs : IpAddress)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](../nada_base_types/string.md)| |
> |port|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function IpAddress(host : String, port : Integer)
> ``` 


---  
 #  IpAddress : Void

 `constructor`

> Creates an empty IP address.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](../nada_base_types/string.md)| |
> |port|[integer](../nada_base_types/integer.md)| |
> |internetProtocol|[InternetProtocol](../enum_reference.md#internetprotocol)| |
> ``` lang=cpp, name=Nada
> function IpAddress(host : String, port : Integer, internetProtocol : InternetProtocol)
> ``` 


---  
 

 
 `Networking`

(NOTE) Manages all the client/server/peer connections .

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#close-void)|[ ConnectionCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#connectioncount-zilch-eng)|[eventobject](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/eventobject.md)| |
|[ CloseConnection](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#closeconnection-void)|[ IncomingConnectionCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#incomingconnectioncount)| | |
|[ Connect](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#connect-void)|[ OutgoingConnectionCount](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#outgoingconnectioncount)| | |
|[ IsConnected](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#isconnected-zilch-engine)| | | |
|[ Listen](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#listen-zilch-engine-docum)| | | |
|[ SendTo](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#sendto-void)| | | |
|[ SendToAll](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#sendtoall-void)| | | |
|[ SendToAllAndSelf](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#sendtoallandself-void)| | | |
|[ SendToAllExcept](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/tcpsocket.md#sendtoallexcept-void)| | | |


 #  Properties


---  
 #  ConnectionCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Get the number of connections we have.
> ``` lang=cpp, name=Nada
> var ConnectionCount : Integer


---  
 #  IncomingConnectionCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Get the number of incoming connections.
> ``` lang=cpp, name=Nada
> var IncomingConnectionCount : Integer


---  
 #  OutgoingConnectionCount : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `read-only`

> Get the number of outgoing connections.
> ``` lang=cpp, name=Nada
> var OutgoingConnectionCount : Integer


---  
 #  Methods


---  
 #  Close : Void

> Close all activity (whether listening or connected to a server).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Close()
> ``` 


---  
 #  CloseConnection : Void

> 
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function CloseConnection(index : Integer)
> ``` 


---  
 #  Connect : Void

> Attempt to connect to a host on the given port.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |port|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Connect(host : String, port : Integer)
> ``` 


---  
 #  IsConnected : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Check if we are currently connected to anyone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsConnected() : Boolean
> ``` 


---  
 #  Listen : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |maxConnections|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Listen(port : Integer, maxConnections : Integer) : Boolean
> ``` 


---  
 #  Listen : [boolean](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/boolean.md)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |maxConnections|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |bindTo|[TcpSocketBind](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/enum_reference.md#tcpsocketbind)| |
> ``` lang=cpp, name=Nada
> function Listen(port : Integer, maxConnections : Integer, bindTo : TcpSocketBind) : Boolean
> ``` 


---  
 #  SendTo : Void

> Send an event to a specific connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[sendableevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sendableevent.md)| |
> |index|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SendTo(eventId : String, event : SendableEvent, index : Integer)
> ``` 


---  
 #  SendToAll : Void

> Send an event to all connections.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[sendableevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sendableevent.md)| |
> ``` lang=cpp, name=Nada
> function SendToAll(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllAndSelf : Void

> Send an event to all connections and dispatch on self.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[sendableevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sendableevent.md)| |
> ``` lang=cpp, name=Nada
> function SendToAllAndSelf(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllExcept : Void

> Send an event to all connections except a particular connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |event|[sendableevent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/sendableevent.md)| |
> |exceptIndex|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SendToAllExcept(eventId : String, event : SendableEvent, exceptIndex : Integer)
> ``` 


---  
 

 
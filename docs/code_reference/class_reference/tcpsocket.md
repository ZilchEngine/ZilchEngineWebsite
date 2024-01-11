 `Networking`

(NOTE) Manages all the client/server/peer connections .

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Close](tcpsocket.md#close-void)|[ ConnectionCount](tcpsocket.md#connectioncount-zilch-eng)|[eventobject](eventobject.md)| |
|[ CloseConnection](tcpsocket.md#closeconnection-void)|[ IncomingConnectionCount](tcpsocket.md#incomingconnectioncount)| | |
|[ Connect](tcpsocket.md#connect-void)|[ OutgoingConnectionCount](tcpsocket.md#outgoingconnectioncount)| | |
|[ IsConnected](tcpsocket.md#isconnected-zilch-engine)| | | |
|[ Listen](tcpsocket.md#listen-zilch-engine-docum)| | | |
|[ SendTo](tcpsocket.md#sendto-void)| | | |
|[ SendToAll](tcpsocket.md#sendtoall-void)| | | |
|[ SendToAllAndSelf](tcpsocket.md#sendtoallandself-void)| | | |
|[ SendToAllExcept](tcpsocket.md#sendtoallexcept-void)| | | |


 #  Properties


---  
 #  ConnectionCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Get the number of connections we have.
> ``` lang=cpp, name=Nada
> var ConnectionCount : Integer


---  
 #  IncomingConnectionCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Get the number of incoming connections.
> ``` lang=cpp, name=Nada
> var IncomingConnectionCount : Integer


---  
 #  OutgoingConnectionCount : [integer](../nada_base_types/integer.md)

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
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function CloseConnection(index : Integer)
> ``` 


---  
 #  Connect : Void

> Attempt to connect to a host on the given port.
> |Name|Type|Description|
> |---|---|---|
> |host|[string](../nada_base_types/string.md)| |
> |port|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Connect(host : String, port : Integer)
> ``` 


---  
 #  IsConnected : [boolean](../nada_base_types/boolean.md)

> Check if we are currently connected to anyone.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function IsConnected() : Boolean
> ``` 


---  
 #  Listen : [boolean](../nada_base_types/boolean.md)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](../nada_base_types/integer.md)| |
> |maxConnections|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Listen(port : Integer, maxConnections : Integer) : Boolean
> ``` 


---  
 #  Listen : [boolean](../nada_base_types/boolean.md)

> Listen for incoming connections.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](../nada_base_types/integer.md)| |
> |maxConnections|[integer](../nada_base_types/integer.md)| |
> |bindTo|[TcpSocketBind](../enum_reference.md#tcpsocketbind)| |
> ``` lang=cpp, name=Nada
> function Listen(port : Integer, maxConnections : Integer, bindTo : TcpSocketBind) : Boolean
> ``` 


---  
 #  SendTo : Void

> Send an event to a specific connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[sendableevent](sendableevent.md)| |
> |index|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SendTo(eventId : String, event : SendableEvent, index : Integer)
> ``` 


---  
 #  SendToAll : Void

> Send an event to all connections.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[sendableevent](sendableevent.md)| |
> ``` lang=cpp, name=Nada
> function SendToAll(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllAndSelf : Void

> Send an event to all connections and dispatch on self.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[sendableevent](sendableevent.md)| |
> ``` lang=cpp, name=Nada
> function SendToAllAndSelf(eventId : String, event : SendableEvent)
> ``` 


---  
 #  SendToAllExcept : Void

> Send an event to all connections except a particular connection index.
> |Name|Type|Description|
> |---|---|---|
> |eventId|[string](../nada_base_types/string.md)| |
> |event|[sendableevent](sendableevent.md)| |
> |exceptIndex|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function SendToAllExcept(eventId : String, event : SendableEvent, exceptIndex : Integer)
> ``` 


---  
 

 
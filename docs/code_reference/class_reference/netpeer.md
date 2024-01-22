 `Component` `Networking`



(NOTE) Network Peer. Acts as a host on the network. Manages network object state and event replication.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddUser](netpeer.md#adduser-zilch-engine-docu)|[BasicHostInfoTimeout](netpeer.md#basichostinfotimeout-zer)|[netobject](netobject.md)| |
|[CancelHostRequests](netpeer.md#cancelhostrequests-void)|[ExtraHostInfoTimeout](netpeer.md#extrahostinfotimeout-zer)| | |
|[ClearHostList](netpeer.md#clearhostlist-void)|[FrameFillSkip](netpeer.md#framefillskip-zilch-engin)| | |
|[ClearHostLists](netpeer.md#clearhostlists-void)|[FrameFillWarning](netpeer.md#framefillwarning-zilch-en)| | |
|[Close](netpeer.md#close-void)|[HostPingInterval](netpeer.md#hostpinginterval-zilch-en)| | |
|[ConnectLink](netpeer.md#connectlink-zilch-engine)|[HostPortRangeEnd](netpeer.md#hostportrangeend-zilch-en)| | |
|[DisconnectAllLinks](netpeer.md#disconnectalllinks-zero)|[HostPortRangeStart](netpeer.md#hostportrangestart-zero)| | |
|[DisconnectLink](netpeer.md#disconnectlink-zilch-engi)|[Info](netpeer.md#info-zilch-engine-documen)| | |
|[DiscoverHostList](netpeer.md#discoverhostlist-zilch-en)|[InternetDiscoverable](netpeer.md#internetdiscoverable-zer)| | |
|[GetHostByAddress](netpeer.md#gethostbyaddress-zilch-en)|[InternetHostListTimeout](netpeer.md#internethostlisttimeout)| | |
|[GetHostByIndex](netpeer.md#gethostbyindex-zilch-engi)|[InternetHostPublishInterval](netpeer.md#internethostpublishinter)| | |
|[GetHostList](netpeer.md#gethostlist-zilch-engine)|[InternetHostRecordLifetime](netpeer.md#internethostrecordlifeti)| | |
|[GetLinkCreationDirection](netpeer.md#getlinkcreationdirection)|[InternetSameIpHostRecordLimit](netpeer.md#internetsameiphostrecord)| | |
|[GetLinkInternetProtocol](netpeer.md#getlinkinternetprotocol)|[Ipv4Address](netpeer.md#ipv4address-zilch-engine)| | |
|[GetLinkIpAddress](netpeer.md#getlinkipaddress-zilch-en)|[Ipv4Host](netpeer.md#ipv4host-zilch-engine-doc)| | |
|[GetLinkNetPeerId](netpeer.md#getlinknetpeerid-zilch-en)|[Ipv4Port](netpeer.md#ipv4port-zilch-engine-doc)| | |
|[GetLinkState](netpeer.md#getlinkstate-zilch-engine)|[IsOpen](netpeer.md#isopen-zilch-engine-docum)| | |
|[GetLinkStatus](netpeer.md#getlinkstatus-zilch-engin)|[LanDiscoverable](netpeer.md#landiscoverable-zilch-eng)| | |
|[GetNetObject](netpeer.md#getnetobject-zilch-engine)|[LinkCount](netpeer.md#linkcount-zilch-engine-do)| | |
|[GetNetSpace](netpeer.md#getnetspace-zilch-engine)|[NetObjectCount](netpeer.md#netobjectcount-zilch-engi)| | |
|[GetOurIpAddressFromLink](netpeer.md#getouripaddressfromlink)|[NetPeerId](netpeer.md#netpeerid-zilch-engine-do)| | |
|[GetUser](netpeer.md#getuser-zilch-engine-docu)|[NetSpaceCount](netpeer.md#netspacecount-zilch-engin)| | |
|[GetUsersAddedByPeer](netpeer.md#getusersaddedbypeer-zero)|[NetUserCount](netpeer.md#netusercount-zilch-engine)| | |
|[Constructor](netpeer.md#netpeer-void)|[UserCount](netpeer.md#usercount-zilch-engine-do)| | |
|[Open](netpeer.md#open-zilch-engine-documen)|[Users](netpeer.md#users-zilch-engine-docume)| | |
|[OpenClient](netpeer.md#openclient-zilch-engine-d)|[UsersAddedByMyPeer](netpeer.md#usersaddedbymypeer-zero)| | |
|[OpenOffline](netpeer.md#openoffline-zilch-engine)| | | |
|[OpenServer](netpeer.md#openserver-zilch-engine-d)| | | |
|[RefreshHost](netpeer.md#refreshhost-zilch-engine)| | | |
|[RefreshHostList](netpeer.md#refreshhostlist-zilch-eng)| | | |
|[RemoveUser](netpeer.md#removeuser-zilch-engine-d)| | | |
|[SubscribeToMasterServer](netpeer.md#subscribetomasterserver)| | | |
|[UnsubscribeFromMasterServer](netpeer.md#unsubscribefrommasterser)| | | |


 #  Properties


---  
 #  BasicHostInfoTimeout : [real](../nada_base_types/real.md)

> [Client/Server] Determines the amount of time the client is willing to wait for.
> ```TS:Nada
> var BasicHostInfoTimeout : Real


---  
 #  ExtraHostInfoTimeout : [real](../nada_base_types/real.md)

> [Client/Server] Determines the amount of time the client will wait for extra host info from a server.
> ```TS:Nada
> var ExtraHostInfoTimeout : Real


---  
 #  FrameFillSkip : [real](../nada_base_types/real.md)

> Controls when to skip change replication for the current frame because of remaining outgoing bandwidth utilization ratio on any given link.
> ```TS:Nada
> var FrameFillSkip : Real


---  
 #  FrameFillWarning : [real](../nada_base_types/real.md)

> Controls when the user will be warned of their current frame's outgoing bandwidth utilization ratio on any given link.
> ```TS:Nada
> var FrameFillWarning : Real


---  
 #  HostPingInterval : [real](../nada_base_types/real.md)

> [Client/Server] The time between (potentially) redundant pings from a net peer.
> ```TS:Nada
> var HostPingInterval : Real


---  
 #  HostPortRangeEnd : [integer](../nada_base_types/integer.md)

> Configures the inclusive range of ports used to host this game.
> ```TS:Nada
> var HostPortRangeEnd : Integer


---  
 #  HostPortRangeStart : [integer](../nada_base_types/integer.md)

> Configures the inclusive range of ports used to host this game.
> ```TS:Nada
> var HostPortRangeStart : Integer


---  
 #  Info : [string](../nada_base_types/string.md)

 `read-only`

> Current peer identifier information display string. Provided for logging and debugging convenience. Contains the peer's local IP address, network role, and net peer ID.
> ```TS:Nada
> var Info : String


---  
 #  InternetDiscoverable : [boolean](../nada_base_types/boolean.md)

> Configures the server peer to be discoverable on the internet.
> ```TS:Nada
> var InternetDiscoverable : Boolean


---  
 #  InternetHostListTimeout : [real](../nada_base_types/real.md)

> [Client/Server] Determines the amount of time the client is willing to wait to get a host list from master server.
> ```TS:Nada
> var InternetHostListTimeout : Real


---  
 #  InternetHostPublishInterval : [real](../nada_base_types/real.md)

> Controls how often the internet discoverable peer sends a host record message to its master server subscriptions.
> ```TS:Nada
> var InternetHostPublishInterval : Real


---  
 #  InternetHostRecordLifetime : [real](../nada_base_types/real.md)

> Controls the lifetime of every host record stored on the master server.
> ```TS:Nada
> var InternetHostRecordLifetime : Real


---  
 #  InternetSameIpHostRecordLimit : [integer](../nada_base_types/integer.md)

> Controls how many host records from the same IP address may be stored on the master server (used to prevent flood attacks).
> ```TS:Nada
> var InternetSameIpHostRecordLimit : Integer


---  
 #  Ipv4Address : [ipaddress](ipaddress.md)

 `read-only`

> Returns the peer's local IPv4 address, else IpAddress(). Set if the peer is open with an IPv4 socket.
> ```TS:Nada
> var Ipv4Address : IpAddress


---  
 #  Ipv4Host : [string](../nada_base_types/string.md)

 `read-only`

> Returns the peer's local IPv4 address host as a numeric address string, else String().
> ```TS:Nada
> var Ipv4Host : String


---  
 #  Ipv4Port : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the peer's local IPv4 address port, else String().
> ```TS:Nada
> var Ipv4Port : Integer


---  
 #  IsOpen : [boolean](../nada_base_types/boolean.md)

 `read-only`

> Returns true if the peer is open, else false.
> ```TS:Nada
> var IsOpen : Boolean


---  
 #  LanDiscoverable : [boolean](../nada_base_types/boolean.md)

> Configures the server peer to be discoverable on the local area network.
> ```TS:Nada
> var LanDiscoverable : Boolean


---  
 #  LinkCount : [integer](../nada_base_types/integer.md)

 `read-only`

> [Client/Server] Returns the number of connected network links managed by this peer.
> ```TS:Nada
> var LinkCount : Integer


---  
 #  NetObjectCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net objects in this game session (but not including the net peer itself).
> ```TS:Nada
> var NetObjectCount : Integer


---  
 #  NetPeerId : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the open peer's unique network identifier, else 0. [Server/Offline] This will always be zero. [Client] This will be non-zero once connected to a server, else zero.
> ```TS:Nada
> var NetPeerId : Integer


---  
 #  NetSpaceCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net spaces in this game session.
> ```TS:Nada
> var NetSpaceCount : Integer


---  
 #  NetUserCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of net users in this game session.
> ```TS:Nada
> var NetUserCount : Integer


---  
 #  UserCount : [integer](../nada_base_types/integer.md)

 `read-only`

> Returns the number of added network users.
> ```TS:Nada
> var UserCount : Integer


---  
 #  Users : [netuserrange](netuserrange.md)

 `read-only`

> Returns all added network users.
> ```TS:Nada
> var Users : NetUserRange


---  
 #  UsersAddedByMyPeer : [netuserrange](netuserrange.md)

 `read-only`

> Returns the network users added by our local peer.
> ```TS:Nada
> var UsersAddedByMyPeer : NetUserRange


---  
 #  Methods


---  
 #  AddUser : [boolean](../nada_base_types/boolean.md)

> Initiates a network user add request to add a new user belonging to our local peer (delayed until end of frame). Listen to the NetUser event interface to handle the results. Returns true if the request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function AddUser() : Boolean
> ``` 


---  
 #  AddUser : [boolean](../nada_base_types/boolean.md)

> Initiates a network user add request to add a new user belonging to our local peer (delayed until end of frame). Listen to the NetUser event interface to handle the results. Returns true if the request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function AddUser(requestEvent : Event) : Boolean
> ``` 


---  
 #  AddUser : [boolean](../nada_base_types/boolean.md)

> Initiates a network user add request to add a new user belonging to our local peer (delayed until end of frame). Listen to the NetUser event interface to handle the results. Returns true if the request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function AddUser(requestBundle : EventBundle) : Boolean
> ``` 


---  
 #  CancelHostRequests : Void

> Cancels all host discovery and refresh requests currently in progress (the operations will be considered unsuccessful). Listen to the NetHost event interface to handle the results.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function CancelHostRequests()
> ``` 


---  
 #  ClearHostList : Void

> Clears the given network's host list.
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> ```TS:Nada
> function ClearHostList(network : Network)
> ``` 


---  
 #  ClearHostLists : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ClearHostLists()
> ``` 


---  
 #  Close : Void

> Closes the peer (safe to call multiple times).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Close()
> ``` 


---  
 #  ConnectLink : [boolean](../nada_base_types/boolean.md)

> [Client] Initiates a connect attempt with the remote peer (delayed until end of frame). Listen to the NetLink event interface to handle the results. Returns true if a connect request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function ConnectLink(ipAddress : IpAddress) : Boolean
> ``` 


---  
 #  ConnectLink : [boolean](../nada_base_types/boolean.md)

> [Client] Initiates a connect attempt with the remote peer (delayed until end of frame). Listen to the NetLink event interface to handle the results. Returns true if a connect request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function ConnectLink(ipAddress : IpAddress, requestEvent : Event) : Boolean
> ``` 


---  
 #  ConnectLink : [boolean](../nada_base_types/boolean.md)

> [Client] Initiates a connect attempt with the remote peer (delayed until end of frame). Listen to the NetLink event interface to handle the results. Returns true if a connect request was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function ConnectLink(ipAddress : IpAddress, requestBundle : EventBundle) : Boolean
> ``` 


---  
 #  DisconnectAllLinks : [integer](../nada_base_types/integer.md)

> [Client/Server] Disconnects by request from all remote peers. Listen to the NetLink event interface to handle the results. Returns the number of links disconnected.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function DisconnectAllLinks() : Integer
> ``` 


---  
 #  DisconnectAllLinks : [integer](../nada_base_types/integer.md)

> [Client/Server] Disconnects by request from all remote peers. Listen to the NetLink event interface to handle the results. Returns the number of links disconnected.
> |Name|Type|Description|
> |---|---|---|
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function DisconnectAllLinks(requestEvent : Event) : Integer
> ``` 


---  
 #  DisconnectAllLinks : [integer](../nada_base_types/integer.md)

> [Client/Server] Disconnects by request from all remote peers. Listen to the NetLink event interface to handle the results. Returns the number of links disconnected.
> |Name|Type|Description|
> |---|---|---|
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function DisconnectAllLinks(requestBundle : EventBundle) : Integer
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function DisconnectLink(netPeerId : Integer) : Boolean
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function DisconnectLink(netPeerId : Integer, requestEvent : Event) : Boolean
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function DisconnectLink(netPeerId : Integer, requestBundle : EventBundle) : Boolean
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function DisconnectLink(ipAddress : IpAddress) : Boolean
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function DisconnectLink(ipAddress : IpAddress, requestEvent : Event) : Boolean
> ``` 


---  
 #  DisconnectLink : [boolean](../nada_base_types/boolean.md)

> [Client/Server] Disconnects by request from the remote peer. Listen to the NetLink event interface to handle the results. Returns true if a disconnect notice was successfully initiated, else false.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function DisconnectLink(ipAddress : IpAddress, requestBundle : EventBundle) : Boolean
> ``` 


---  
 #  DiscoverHostList : [boolean](../nada_base_types/boolean.md)

> Discovers the given network's host list. Listen to the NetHost event interface to handle the results. Returns true if the discovery was successfully started, else false.
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> |removeStaleHosts|[boolean](../nada_base_types/boolean.md)| |
> ```TS:Nada
> function DiscoverHostList(network : Network, removeStaleHosts : Boolean) : Boolean
> ``` 


---  
 #  GetHostByAddress : [nethost](nethost.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function GetHostByAddress(ipAddress : IpAddress) : NetHost
> ``` 


---  
 #  GetHostByAddress : [nethost](nethost.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function GetHostByAddress(network : Network, ipAddress : IpAddress) : NetHost
> ``` 


---  
 #  GetHostByIndex : [nethost](nethost.md)

> Returns the first equivalent host found in the given network's host list, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetHostByIndex(network : Network, index : Integer) : NetHost
> ``` 


---  
 #  GetHostList : [nethostrange](nethostrange.md)

> Returns the given network's host list.
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> ```TS:Nada
> function GetHostList(network : Network) : NetHostRange
> ``` 


---  
 #  GetLinkCreationDirection : [TransmissionDirection](../enum_reference.md#transmissiondirection)

> [Client/Server] Returns the direction in which the link was created (which peer initiated the connection), else TransmissionDirection::Unspecified.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetLinkCreationDirection(netPeerId : Integer) : TransmissionDirection
> ``` 


---  
 #  GetLinkInternetProtocol : [InternetProtocol](../enum_reference.md#internetprotocol)

> [Client/Server] Returns the link's IP address protocol version, else InternetProtocol::Unspecified. This IP address protocol will never change for the lifetime of this link.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetLinkInternetProtocol(netPeerId : Integer) : InternetProtocol
> ``` 


---  
 #  GetLinkIpAddress : [ipaddress](ipaddress.md)

> [Client/Server] Returns the remote peer's IP address (as seen from our perspective), else IpAddress(). For outgoing links this is the same IP address specified in our connect call. This IP address will never change for the lifetime of this link.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetLinkIpAddress(netPeerId : Integer) : IpAddress
> ``` 


---  
 #  GetLinkNetPeerId : [integer](../nada_base_types/integer.md)

> Returns the remote peer's unique network identifier, else 0. [Server] This will be non-zero if the client is connected, else zero. [Client] This will always be zero.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function GetLinkNetPeerId(ipAddress : IpAddress) : Integer
> ``` 


---  
 #  GetLinkState : [LinkState](../enum_reference.md#linkstate)

> [Client/Server] Returns the link's specific state, else LinkState::Unspecified.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetLinkState(netPeerId : Integer) : LinkState
> ``` 


---  
 #  GetLinkStatus : [LinkStatus](../enum_reference.md#linkstatus)

> [Client/Server] Returns the link's overall status, else LinkStatus::Unspecified.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetLinkStatus(netPeerId : Integer) : LinkStatus
> ``` 


---  
 #  GetNetObject : [cog](cog.md)

> Returns the live net object specified if it is known locally, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netObjectId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetNetObject(netObjectId : Integer) : Cog
> ``` 


---  
 #  GetNetSpace : [space](space.md)

> Returns the live net space specified if it is known locally, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netObjectId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetNetSpace(netObjectId : Integer) : Space
> ``` 


---  
 #  GetOurIpAddressFromLink : [ipaddress](ipaddress.md)

> [Client/Server] Returns our peer's IP address (as seen from their perspective), else IpAddress(). For incoming links this is the same IP address specified in their connect call. (Available if the link is connected or incoming and attempting connection) It is absolutely possible that this does not match our local IP address.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetOurIpAddressFromLink(netPeerId : Integer) : IpAddress
> ``` 


---  
 #  GetUser : [cog](cog.md)

> Returns the specified network user, else nullptr.
> |Name|Type|Description|
> |---|---|---|
> |netUserId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetUser(netUserId : Integer) : Cog
> ``` 


---  
 #  GetUsersAddedByPeer : [netuserrange](netuserrange.md)

> Returns the network users added by the specified peer.
> |Name|Type|Description|
> |---|---|---|
> |netPeerId|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function GetUsersAddedByPeer(netPeerId : Integer) : NetUserRange
> ``` 


---  
 #  NetPeer : Void

 `constructor`

> Constructor.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function NetPeer()
> ``` 


---  
 #  Open : [boolean](../nada_base_types/boolean.md)

> Opens the peer with the specified network role on any available port. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |role|[NetRole](../enum_reference.md#netrole)| |
> ```TS:Nada
> function Open(role : NetRole) : Boolean
> ``` 


---  
 #  Open : [boolean](../nada_base_types/boolean.md)

> Opens the peer with the specified network role and port settings. Specify port 0 to indicate any available port should be used. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |role|[NetRole](../enum_reference.md#netrole)| |
> |port|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Open(role : NetRole, port : Integer) : Boolean
> ``` 


---  
 #  Open : [boolean](../nada_base_types/boolean.md)

> Opens the peer with the specified network role, port, and retry settings. For the given number of retries, if binding is unsuccessful, the port number is incremented and binding is attempted again. Specify port 0 to indicate any available port should be used. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |role|[NetRole](../enum_reference.md#netrole)| |
> |port|[integer](../nada_base_types/integer.md)| |
> |retries|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Open(role : NetRole, port : Integer, retries : Integer) : Boolean
> ``` 


---  
 #  OpenClient : [boolean](../nada_base_types/boolean.md)

> Opens the peer as a client on any available port. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function OpenClient() : Boolean
> ``` 


---  
 #  OpenClient : [boolean](../nada_base_types/boolean.md)

> Opens the peer as a client with the specified network port. Specify port 0 to indicate any available port should be used. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function OpenClient(port : Integer) : Boolean
> ``` 


---  
 #  OpenClient : [boolean](../nada_base_types/boolean.md)

> Opens the peer as a client with the specified network port and retry settings. For the given number of retries, if binding is unsuccessful, the port number is incremented and binding is attempted again. Specify port 0 to indicate any available port should be used. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](../nada_base_types/integer.md)| |
> |retries|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function OpenClient(port : Integer, retries : Integer) : Boolean
> ``` 


---  
 #  OpenOffline : [boolean](../nada_base_types/boolean.md)

> Opens the peer in offline mode. In offline mode, the peer will act as a pass-through and simulate all applicable network events locally. Always succeeds and returns true.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function OpenOffline() : Boolean
> ``` 


---  
 #  OpenServer : [boolean](../nada_base_types/boolean.md)

> Opens the peer as a server on any available port. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function OpenServer() : Boolean
> ``` 


---  
 #  OpenServer : [boolean](../nada_base_types/boolean.md)

> Opens the peer as a server with the specified network port. Specify port 0 to indicate any available port should be used. Returns true if successful, else false.
> |Name|Type|Description|
> |---|---|---|
> |port|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function OpenServer(port : Integer) : Boolean
> ``` 


---  
 #  RefreshHost : [boolean](../nada_base_types/boolean.md)

> Refreshes the specified host in the given network's host list. Allowing discovery will enable the host to be discovered if it is not an already known host. Listen to the NetHost event interface to handle the results. Returns true if the host was found and the refresh successfully started, else false (the host could not be found).
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> |ipAddress|[ipaddress](ipaddress.md)| |
> |getExtraHostInfo|[boolean](../nada_base_types/boolean.md)| |
> |allowDiscovery|[boolean](../nada_base_types/boolean.md)| |
> |removeStaleHosts|[boolean](../nada_base_types/boolean.md)| |
> ```TS:Nada
> function RefreshHost(network : Network, ipAddress : IpAddress, getExtraHostInfo : Boolean, allowDiscovery : Boolean, removeStaleHosts : Boolean) : Boolean
> ``` 


---  
 #  RefreshHostList : [boolean](../nada_base_types/boolean.md)

> Refreshes all hosts in the given network's host list. Allowing discovery will enable new hosts to be discovered in the process of refreshing. Listen to the NetHost event interface to handle the results. Returns true if the refresh was successfully started, else false.
> |Name|Type|Description|
> |---|---|---|
> |network|[Network](../enum_reference.md#network)| |
> |getExtraHostInfo|[boolean](../nada_base_types/boolean.md)| |
> |allowDiscovery|[boolean](../nada_base_types/boolean.md)| |
> |removeStaleHosts|[boolean](../nada_base_types/boolean.md)| |
> ```TS:Nada
> function RefreshHostList(network : Network, getExtraHostInfo : Boolean, allowDiscovery : Boolean, removeStaleHosts : Boolean) : Boolean
> ``` 


---  
 #  RemoveUser : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> ```TS:Nada
> function RemoveUser(cog : Cog) : Boolean
> ``` 


---  
 #  RemoveUser : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> |requestEvent|[event](event.md)| |
> ```TS:Nada
> function RemoveUser(cog : Cog, requestEvent : Event) : Boolean
> ``` 


---  
 #  RemoveUser : [boolean](../nada_base_types/boolean.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |cog|[cog](cog.md)| |
> |requestBundle|[eventbundle](eventbundle.md)| |
> ```TS:Nada
> function RemoveUser(cog : Cog, requestBundle : EventBundle) : Boolean
> ``` 


---  
 #  SubscribeToMasterServer : Void

> Subscribes to the master server located at the specified IP address. All internet host discovery, record publishing, connection facilitation (NAT punch-through) requests are performed on these master server subscriptions in the order they were subscribed.
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function SubscribeToMasterServer(ipAddress : IpAddress)
> ``` 


---  
 #  UnsubscribeFromMasterServer : Void

> Unsubscribes from the master server located at the specified IP address (if subscribed).
> |Name|Type|Description|
> |---|---|---|
> |ipAddress|[ipaddress](ipaddress.md)| |
> ```TS:Nada
> function UnsubscribeFromMasterServer(ipAddress : IpAddress)
> ``` 


---  
 

 
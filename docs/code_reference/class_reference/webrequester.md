 `Component` `Networking`



(NOTE) A component we can use to facilitate web requests.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Clear](webrequester.md#clear-void)|[Url](webrequester.md#url-zilch-engine-document)|[component](component.md)| |
|[Run](webrequester.md#run-void)| | | |
|[SetHeader](webrequester.md#setheader-void)| | | |
|[SetPostData](webrequester.md#setpostdata-void)| | | |
|[Constructor](webrequester.md#webrequester-void)| | | |


 #  Properties


---  
 #  Url : [string](../nada_base_types/string.md)

> Get and set the url that we make requests to.
> ```TS:Nada
> var Url : String


---  
 #  Methods


---  
 #  Clear : Void

> Clear headers and post data.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Clear()
> ``` 


---  
 #  Run : Void

> Run the web request (we should get data back in a WebResponse event).
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Run()
> ``` 


---  
 #  SetHeader : Void

> Add a header to the web request .
> |Name|Type|Description|
> |---|---|---|
> |name|[string](../nada_base_types/string.md)| |
> |data|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function SetHeader(name : String, data : String)
> ``` 


---  
 #  SetPostData : Void

> Add Post data to the request, this will also change the request to a post request.
> |Name|Type|Description|
> |---|---|---|
> |data|[string](../nada_base_types/string.md)| |
> ```TS:Nada
> function SetPostData(data : String)
> ``` 


---  
 #  WebRequester : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function WebRequester()
> ``` 


---  
 

 
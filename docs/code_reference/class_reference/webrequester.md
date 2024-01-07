 `Component` `Networking`



(NOTE) A component we can use to facilitate web requests.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Clear](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#clear-void)|[ Url](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#url-zilch-engine-document)|[component](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/component.md)| |
|[ Run](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#run-void)| | | |
|[ SetHeader](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#setheader-void)| | | |
|[ SetPostData](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#setpostdata-void)| | | |
|[ Constructor](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/class_reference/webrequester.md#webrequester-void)| | | |


 #  Properties


---  
 #  Url : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

> Get and set the url that we make requests to.
> ``` lang=cpp, name=Nada
> var Url : String


---  
 #  Methods


---  
 #  Clear : Void

> Clear headers and post data.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Run : Void

> Run the web request (we should get data back in a WebResponse event).
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Run()
> ``` 


---  
 #  SetHeader : Void

> Add a header to the web request .
> |Name|Type|Description|
> |---|---|---|
> |name|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> |data|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function SetHeader(name : String, data : String)
> ``` 


---  
 #  SetPostData : Void

> Add Post data to the request, this will also change the request to a post request.
> |Name|Type|Description|
> |---|---|---|
> |data|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function SetPostData(data : String)
> ``` 


---  
 #  WebRequester : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function WebRequester()
> ``` 


---  
 

 
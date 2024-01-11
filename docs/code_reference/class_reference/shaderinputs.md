 `Graphics`

(NOTE) A set of shader inputs for overriding values per object or globally.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Add](shaderinputs.md#add-void)| |[referencecountedthreadsafeid32](referencecountedthreadsafeid32.md)| |
|[ Clear](shaderinputs.md#clear-void)| | | |
|[ Remove](shaderinputs.md#remove-void)| | | |
|[ Constructor](shaderinputs.md#shaderinputs-void)| | | |


 #  Properties


---  
 #  Methods


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[boolean](../nada_base_types/boolean.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Boolean)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[integer](../nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Integer)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ||[string](../nada_base_types/string.md)| |
> ||[integer2](../nada_base_types/integer2.md)| |
> ``` lang=cpp, name=Nada
> function Add( : String,  : String,  : Integer2)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ||[string](../nada_base_types/string.md)| |
> ||[integer3](../nada_base_types/integer3.md)| |
> ``` lang=cpp, name=Nada
> function Add( : String,  : String,  : Integer3)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ||[string](../nada_base_types/string.md)| |
> ||[integer4](../nada_base_types/integer4.md)| |
> ``` lang=cpp, name=Nada
> function Add( : String,  : String,  : Integer4)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[real](../nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Real)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[real2](../nada_base_types/real2.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Real2)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[real3](../nada_base_types/real3.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Real3)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ||[string](../nada_base_types/string.md)| |
> ||[real3x3](../nada_base_types/real3x3.md)| |
> ``` lang=cpp, name=Nada
> function Add( : String,  : String,  : Real3x3)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[real4](../nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Real4)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> ||[string](../nada_base_types/string.md)| |
> ||[string](../nada_base_types/string.md)| |
> ||[real4x4](../nada_base_types/real4x4.md)| |
> ``` lang=cpp, name=Nada
> function Add( : String,  : String,  : Real4x4)
> ``` 


---  
 #  Add : Void

> Add an input value for a specific fragment.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> |input|[texture](texture.md)| |
> ``` lang=cpp, name=Nada
> function Add(fragmentName : String, inputName : String, input : Texture)
> ``` 


---  
 #  Clear : Void

> Remove all added inputs.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Clear()
> ``` 


---  
 #  Remove : Void

> Remove a specific input that was added.
> |Name|Type|Description|
> |---|---|---|
> |fragmentName|[string](../nada_base_types/string.md)| |
> |inputName|[string](../nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function Remove(fragmentName : String, inputName : String)
> ``` 


---  
 #  ShaderInputs : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ShaderInputs()
> ``` 


---  
 #  ShaderInputs : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ||[shaderinputs](shaderinputs.md)| |
> ``` lang=cpp, name=Nada
> function ShaderInputs( : ShaderInputs)
> ``` 


---  
 

 
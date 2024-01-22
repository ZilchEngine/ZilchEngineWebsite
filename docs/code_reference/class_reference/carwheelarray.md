 `Physics`

(NOTE) An array interface to the cog paths of wheels that this car uses. This array is read-only.

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Get](carwheelarray.md#get-zilch-engine-document)|[Count](carwheelarray.md#count-zilch-engine-docume)|[safeid32object](safeid32object.md)| |


 #  Properties


---  
 #  Count : [integer](../nada_base_types/integer.md)

 `read-only`

> How many wheels this car owns.
> ```TS:Nada
> var Count : Integer


---  
 #  Methods


---  
 #  Get : [cog](cog.md)

> Get the cog for a wheel by index.
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](../nada_base_types/integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : Cog
> ``` 


---  
 

 
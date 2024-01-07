 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ FromBytes](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#frombytes-zilch-engine-do)| | | |
|[ FromHexString](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#fromhexstring-zilch-engin)| | | |
|[ FromHsva](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#fromhsva-zilch-engine-doc)| | | |
|[ FromInteger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#frominteger-zilch-engine)| | | |
|[ ToBytes](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#tobytes-zilch-engine-docu)| | | |
|[ ToHexString](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#tohexstring-zilch-engine)| | | |
|[ ToHsva](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#tohsva-zilch-engine-docum)| | | |
|[ ToInteger](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/color.md#tointeger-zilch-engine-do)| | | |


 #  Properties


---  
 #  Methods


---  
 #  FromBytes : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts RGB Bytes [0-255] into an RGBA Real4 (alpha defaults to 1.0). Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |g|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |b|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function FromBytes(r : Integer, g : Integer, b : Integer) : Real4
> ``` 


---  
 #  FromBytes : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts RGBA Bytes [0-255] into an RGBA Real4. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |g|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |b|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |a|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function FromBytes(r : Integer, g : Integer, b : Integer, a : Integer) : Real4
> ``` 


---  
 #  FromBytes : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts RGBA Bytes [0-255] into an RGBA Real4. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[integer4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer4.md)| |
> ``` lang=cpp, name=Nada
> function FromBytes(rgba : Integer4) : Real4
> ``` 


---  
 #  FromHexString : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts a hex String into an RGBA Real4. Must be a 3, 4, 6, or 8 digit RGB[A] representation with an optional preceding '#' or '0x' (case insensitive). E.g. #f00, #F00F, ff0000, 0x00FF00FF.
> |Name|Type|Description|
> |---|---|---|
> |value|[string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)| |
> ``` lang=cpp, name=Nada
> function FromHexString(value : String) : Real4
> ``` 


---  
 #  FromHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts HSV Reals into an RGBA Real4 (alpha defaults to 1.0). The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |h|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |s|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |v|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function FromHsva(h : Real, s : Real, v : Real) : Real4
> ``` 


---  
 #  FromHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts HSVA Reals into an RGBA Real4. The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |h|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |s|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |v|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function FromHsva(h : Real, s : Real, v : Real, a : Real) : Real4
> ``` 


---  
 #  FromHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts an HSVA Real4 into an RGBA Real4. The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |hsva|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function FromHsva(hsva : Real4) : Real4
> ``` 


---  
 #  FromInteger : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts an RGBA packed Integer into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function FromInteger(rgba : Integer) : Real4
> ``` 


---  
 #  FromInteger : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts an RGB packed Integer and an alpha Byte [0-255] into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgb|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |a|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> ``` lang=cpp, name=Nada
> function FromInteger(rgb : Integer, a : Integer) : Real4
> ``` 


---  
 #  FromInteger : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts an RGB packed Integer and an alpha Real into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgb|[integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function FromInteger(rgb : Integer, a : Real) : Real4
> ``` 


---  
 #  ToBytes : [integer4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer4.md)

 `static`

> Converts RGB Reals into an RGBA Integer4 [0-255] (alpha defaults to 255). Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToBytes(r : Real, g : Real, b : Real) : Integer4
> ``` 


---  
 #  ToBytes : [integer4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer4.md)

 `static`

> Converts RGBA Reals into an RGBA Integer4 [0-255]. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToBytes(r : Real, g : Real, b : Real, a : Real) : Integer4
> ``` 


---  
 #  ToBytes : [integer4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer4.md)

 `static`

> Converts an RGBA Real4 into an RGBA Integer4 [0-255]. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function ToBytes(rgba : Real4) : Integer4
> ``` 


---  
 #  ToHexString : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `static`

> Converts RGB Reals into the 8 digit hex format RRGGBBAA (alpha defaults to 1.0 so the end will always be FF).
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToHexString(r : Real, g : Real, b : Real) : String
> ``` 


---  
 #  ToHexString : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `static`

> Converts RGBA Reals into the 8 digit hex format RRGGBBAA.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToHexString(r : Real, g : Real, b : Real, a : Real) : String
> ``` 


---  
 #  ToHexString : [string](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/string.md)

 `static`

> Converts an RGBA Real4 into the 8 digit hex format RRGGBBAA.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function ToHexString(rgba : Real4) : String
> ``` 


---  
 #  ToHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts RGB Reals into an HSVA Real4 (alpha defaults to 1.0).
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToHsva(r : Real, g : Real, b : Real) : Real4
> ``` 


---  
 #  ToHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts RGBA Reals into an HSVA Real4.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToHsva(r : Real, g : Real, b : Real, a : Real) : Real4
> ``` 


---  
 #  ToHsva : [real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)

 `static`

> Converts an RGBA Real4 into an HSVA Real4.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function ToHsva(rgba : Real4) : Real4
> ``` 


---  
 #  ToInteger : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> Converts RGB Reals into an RGBA packed Integer (alpha defaults to 255). Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToInteger(r : Real, g : Real, b : Real) : Integer
> ``` 


---  
 #  ToInteger : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> Converts RGBA Reals into an RGBA packed Integer. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |g|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |b|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> |a|[real](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real.md)| |
> ``` lang=cpp, name=Nada
> function ToInteger(r : Real, g : Real, b : Real, a : Real) : Integer
> ``` 


---  
 #  ToInteger : [integer](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/integer.md)

 `static`

> Converts an RGBA Real4 into an RGBA packed Integer. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/nada_base_types/real4.md)| |
> ``` lang=cpp, name=Nada
> function ToInteger(rgba : Real4) : Integer
> ``` 


---  
 

 
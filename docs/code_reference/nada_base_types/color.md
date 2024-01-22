 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[FromBytes](color.md#frombytes-zilch-engine-do)| | | |
|[FromHexString](color.md#fromhexstring-zilch-engin)| | | |
|[FromHsva](color.md#fromhsva-zilch-engine-doc)| | | |
|[FromInteger](color.md#frominteger-zilch-engine)| | | |
|[ToBytes](color.md#tobytes-zilch-engine-docu)| | | |
|[ToHexString](color.md#tohexstring-zilch-engine)| | | |
|[ToHsva](color.md#tohsva-zilch-engine-docum)| | | |
|[ToInteger](color.md#tointeger-zilch-engine-do)| | | |


 #  Properties


---  
 #  Methods


---  
 #  FromBytes : [real4](real4.md)

 `static`

> Converts RGB Bytes [0-255] into an RGBA Real4 (alpha defaults to 1.0). Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[integer](integer.md)| |
> |g|[integer](integer.md)| |
> |b|[integer](integer.md)| |
> ```TS:Nada
> function FromBytes(r : Integer, g : Integer, b : Integer) : Real4
> ``` 


---  
 #  FromBytes : [real4](real4.md)

 `static`

> Converts RGBA Bytes [0-255] into an RGBA Real4. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[integer](integer.md)| |
> |g|[integer](integer.md)| |
> |b|[integer](integer.md)| |
> |a|[integer](integer.md)| |
> ```TS:Nada
> function FromBytes(r : Integer, g : Integer, b : Integer, a : Integer) : Real4
> ``` 


---  
 #  FromBytes : [real4](real4.md)

 `static`

> Converts RGBA Bytes [0-255] into an RGBA Real4. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[integer4](integer4.md)| |
> ```TS:Nada
> function FromBytes(rgba : Integer4) : Real4
> ``` 


---  
 #  FromHexString : [real4](real4.md)

 `static`

> Converts a hex String into an RGBA Real4. Must be a 3, 4, 6, or 8 digit RGB[A] representation with an optional preceding '#' or '0x' (case insensitive). E.g. #f00, #F00F, ff0000, 0x00FF00FF.
> |Name|Type|Description|
> |---|---|---|
> |value|[string](string.md)| |
> ```TS:Nada
> function FromHexString(value : String) : Real4
> ``` 


---  
 #  FromHsva : [real4](real4.md)

 `static`

> Converts HSV Reals into an RGBA Real4 (alpha defaults to 1.0). The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |h|[real](real.md)| |
> |s|[real](real.md)| |
> |v|[real](real.md)| |
> ```TS:Nada
> function FromHsva(h : Real, s : Real, v : Real) : Real4
> ``` 


---  
 #  FromHsva : [real4](real4.md)

 `static`

> Converts HSVA Reals into an RGBA Real4. The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |h|[real](real.md)| |
> |s|[real](real.md)| |
> |v|[real](real.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function FromHsva(h : Real, s : Real, v : Real, a : Real) : Real4
> ``` 


---  
 #  FromHsva : [real4](real4.md)

 `static`

> Converts an HSVA Real4 into an RGBA Real4. The hue parameter will wrap if is beyond [0-1]. The saturation and value parameters may go beyond [0-1] to represent HDR values.
> |Name|Type|Description|
> |---|---|---|
> |hsva|[real4](real4.md)| |
> ```TS:Nada
> function FromHsva(hsva : Real4) : Real4
> ``` 


---  
 #  FromInteger : [real4](real4.md)

 `static`

> Converts an RGBA packed Integer into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[integer](integer.md)| |
> ```TS:Nada
> function FromInteger(rgba : Integer) : Real4
> ``` 


---  
 #  FromInteger : [real4](real4.md)

 `static`

> Converts an RGB packed Integer and an alpha Byte [0-255] into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgb|[integer](integer.md)| |
> |a|[integer](integer.md)| |
> ```TS:Nada
> function FromInteger(rgb : Integer, a : Integer) : Real4
> ``` 


---  
 #  FromInteger : [real4](real4.md)

 `static`

> Converts an RGB packed Integer and an alpha Real into an RGBA Real4. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgb|[integer](integer.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function FromInteger(rgb : Integer, a : Real) : Real4
> ``` 


---  
 #  ToBytes : [integer4](integer4.md)

 `static`

> Converts RGB Reals into an RGBA Integer4 [0-255] (alpha defaults to 255). Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> ```TS:Nada
> function ToBytes(r : Real, g : Real, b : Real) : Integer4
> ``` 


---  
 #  ToBytes : [integer4](integer4.md)

 `static`

> Converts RGBA Reals into an RGBA Integer4 [0-255]. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function ToBytes(r : Real, g : Real, b : Real, a : Real) : Integer4
> ``` 


---  
 #  ToBytes : [integer4](integer4.md)

 `static`

> Converts an RGBA Real4 into an RGBA Integer4 [0-255]. Integer is used in place of Byte for convenience.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](real4.md)| |
> ```TS:Nada
> function ToBytes(rgba : Real4) : Integer4
> ``` 


---  
 #  ToHexString : [string](string.md)

 `static`

> Converts RGB Reals into the 8 digit hex format RRGGBBAA (alpha defaults to 1.0 so the end will always be FF).
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> ```TS:Nada
> function ToHexString(r : Real, g : Real, b : Real) : String
> ``` 


---  
 #  ToHexString : [string](string.md)

 `static`

> Converts RGBA Reals into the 8 digit hex format RRGGBBAA.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function ToHexString(r : Real, g : Real, b : Real, a : Real) : String
> ``` 


---  
 #  ToHexString : [string](string.md)

 `static`

> Converts an RGBA Real4 into the 8 digit hex format RRGGBBAA.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](real4.md)| |
> ```TS:Nada
> function ToHexString(rgba : Real4) : String
> ``` 


---  
 #  ToHsva : [real4](real4.md)

 `static`

> Converts RGB Reals into an HSVA Real4 (alpha defaults to 1.0).
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> ```TS:Nada
> function ToHsva(r : Real, g : Real, b : Real) : Real4
> ``` 


---  
 #  ToHsva : [real4](real4.md)

 `static`

> Converts RGBA Reals into an HSVA Real4.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function ToHsva(r : Real, g : Real, b : Real, a : Real) : Real4
> ``` 


---  
 #  ToHsva : [real4](real4.md)

 `static`

> Converts an RGBA Real4 into an HSVA Real4.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](real4.md)| |
> ```TS:Nada
> function ToHsva(rgba : Real4) : Real4
> ``` 


---  
 #  ToInteger : [integer](integer.md)

 `static`

> Converts RGB Reals into an RGBA packed Integer (alpha defaults to 255). Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> ```TS:Nada
> function ToInteger(r : Real, g : Real, b : Real) : Integer
> ``` 


---  
 #  ToInteger : [integer](integer.md)

 `static`

> Converts RGBA Reals into an RGBA packed Integer. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |r|[real](real.md)| |
> |g|[real](real.md)| |
> |b|[real](real.md)| |
> |a|[real](real.md)| |
> ```TS:Nada
> function ToInteger(r : Real, g : Real, b : Real, a : Real) : Integer
> ``` 


---  
 #  ToInteger : [integer](integer.md)

 `static`

> Converts an RGBA Real4 into an RGBA packed Integer. Endianness is handled so that 0x00FF00FF always means full green and full alpha.
> |Name|Type|Description|
> |---|---|---|
> |rgba|[real4](real4.md)| |
> ```TS:Nada
> function ToInteger(rgba : Real4) : Integer
> ``` 


---  
 

 
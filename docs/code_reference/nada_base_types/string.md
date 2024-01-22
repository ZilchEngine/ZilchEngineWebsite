 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[Compare](string.md#compare-zilch-engine-docu)|[All](string.md#all-zilch-engine-document)| | |
|[CompareTo](string.md#compareto-zilch-engine-do)|[Begin](string.md#begin-zilch-engine-docume)| | |
|[ComputeRuneCount](string.md#computerunecount-zilch-en)|[ByteCount](string.md#bytecount-zilch-engine-do)| | |
|[Concatenate](string.md#concatenate-zilch-engine)|[Count](string.md#count-zilch-engine-docume)| | |
|[Contains](string.md#contains-zilch-engine-doc)|[Empty](string.md#empty-zilch-engine-docume)| | |
|[EndsWith](string.md#endswith-zilch-engine-doc)|[End](string.md#end-zilch-engine-document)| | |
|[FindFirstOf](string.md#findfirstof-zilch-engine)|[IsNotEmpty](string.md#isnotempty-zilch-engine-d)| | |
|[FindLastOf](string.md#findlastof-zilch-engine-d)| | | |
|[FindRangeExclusive](string.md#findrangeexclusive-zero)| | | |
|[FindRangeInclusive](string.md#findrangeinclusive-zero)| | | |
|[FormatC](string.md#formatc-zilch-engine-docu)| | | |
|[FromRune](string.md#fromrune-zilch-engine-doc)| | | |
|[Get](string.md#get-zilch-engine-document)| | | |
|[IsNullOrEmpty](string.md#isnullorempty-zilch-engin)| | | |
|[IsNullOrWhitespace](string.md#isnullorwhitespace-zero)| | | |
|[Join](string.md#join-zilch-engine-documen)| | | |
|[Replace](string.md#replace-zilch-engine-docu)| | | |
|[RuneIteratorFromByteIndex](string.md#runeiteratorfrombyteinde)| | | |
|[RuneIteratorFromRuneIndex](string.md#runeiteratorfromruneinde)| | | |
|[Split](string.md#split-zilch-engine-docume)| | | |
|[StartsWith](string.md#startswith-zilch-engine-d)| | | |
|[SubString](string.md#substring-zilch-engine-do)| | | |
|[SubStringBytes](string.md#substringbytes-zilch-engi)| | | |
|[SubStringFromRuneIndices](string.md#substringfromruneindices)| | | |
|[ToLower](string.md#tolower-zilch-engine-docu)| | | |
|[ToUpper](string.md#toupper-zilch-engine-docu)| | | |
|[Trim](string.md#trim-zilch-engine-documen)| | | |
|[TrimEnd](string.md#trimend-zilch-engine-docu)| | | |
|[TrimStart](string.md#trimstart-zilch-engine-do)| | | |


 #  Properties


---  
 #  All : [stringrange](stringrange.md)

 `read-only`

> Converts the string into a string range.
> ```TS:Nada
> var All : StringRange


---  
 #  Begin : [runeiterator](runeiterator.md)

 `read-only`

> Returns the RuneIterator at the start of this string.
> ```TS:Nada
> var Begin : RuneIterator


---  
 #  ByteCount : [integer](integer.md)

 `read-only`

> Returns the number of bytes in the string.
> ```TS:Nada
> var ByteCount : Integer


---  
 #  Count : [integer](integer.md)

 `read-only`

> Returns the number of bytes in the string.
> ```TS:Nada
> var Count : Integer


---  
 #  Empty : [boolean](boolean.md)

 `read-only`

> Returns true if the string is emtpy.
> ```TS:Nada
> var Empty : Boolean


---  
 #  End : [runeiterator](runeiterator.md)

 `read-only`

> Returns the RuneIterator at the end (one past the last Rune) of this string.
> ```TS:Nada
> var End : RuneIterator


---  
 #  IsNotEmpty : [boolean](boolean.md)

 `read-only`

> Returns true if the string is not empty.
> ```TS:Nada
> var IsNotEmpty : Boolean


---  
 #  Methods


---  
 #  Compare : [integer](integer.md)

 `static`

> Compares the two strings and returns an integer to denote their relative sort order.
> |Name|Type|Description|
> |---|---|---|
> |left|[string](string.md)| |
> |right|[string](string.md)| |
> ```TS:Nada
> function Compare(left : String, right : String) : Integer
> ``` 


---  
 #  CompareTo : [integer](integer.md)

> Compares this string to the given string and returns an integer to denote their relative sort order.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function CompareTo(p0 : StringRange) : Integer
> ``` 


---  
 #  ComputeRuneCount : [integer](integer.md)

> Compute the number of runes in the string.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ComputeRuneCount() : Integer
> ``` 


---  
 #  Concatenate : [string](string.md)

 `static`

> Combines the two strings into a new string.
> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> |p1|[string](string.md)| |
> ```TS:Nada
> function Concatenate(p0 : String, p1 : String) : String
> ``` 


---  
 #  Concatenate : [string](string.md)

 `static`

> Combines the two string ranges into a new string.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> |p1|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Concatenate(p0 : StringRange, p1 : StringRange) : String
> ``` 


---  
 #  Contains : [boolean](boolean.md)

> Returns if the string Contains the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Contains(p0 : StringRange) : Boolean
> ``` 


---  
 #  EndsWith : [boolean](boolean.md)

> Returns if the string ends with the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function EndsWith(p0 : StringRange) : Boolean
> ``` 


---  
 #  FindFirstOf : [stringrange](stringrange.md)

> Returns a StringRange that Contains the first occurrence of given StringRange.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function FindFirstOf(p0 : StringRange) : StringRange
> ``` 


---  
 #  FindLastOf : [stringrange](stringrange.md)

> Returns a StringRange that Contains the last occurrence of given StringRange.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function FindLastOf(p0 : StringRange) : StringRange
> ``` 


---  
 #  FindRangeExclusive : [stringrange](stringrange.md)

> Finds the first StringRange that starts with 'startRange' and ends with 'endRange'. This substring excludes 'startRange' and 'endRange'.
> |Name|Type|Description|
> |---|---|---|
> |startRange|[stringrange](stringrange.md)| |
> |endRange|[stringrange](stringrange.md)| |
> ```TS:Nada
> function FindRangeExclusive(startRange : StringRange, endRange : StringRange) : StringRange
> ``` 


---  
 #  FindRangeInclusive : [stringrange](stringrange.md)

> Finds the first StringRange that starts with 'startRange' and ends with 'endRange'. This substring includes 'startRange' and 'endRange'.
> |Name|Type|Description|
> |---|---|---|
> |startRange|[stringrange](stringrange.md)| |
> |endRange|[stringrange](stringrange.md)| |
> ```TS:Nada
> function FindRangeInclusive(startRange : StringRange, endRange : StringRange) : StringRange
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> |p6|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T, p6 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> |p6|T| |
> |p7|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T, p6 : T, p7 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> |p6|T| |
> |p7|T| |
> |p8|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T, p6 : T, p7 : T, p8 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> |p6|T| |
> |p7|T| |
> |p8|T| |
> |p9|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T, p6 : T, p7 : T, p8 : T, p9 : T) : String
> ``` 


---  
 #  FormatC : [string](string.md)

 `static`

> 
> |Name|Type|Description|
> |---|---|---|
> |format|[string](string.md)| |
> |p1|T| |
> |p2|T| |
> |p3|T| |
> |p4|T| |
> |p5|T| |
> |p6|T| |
> |p7|T| |
> |p8|T| |
> |p9|T| |
> |p10|T| |
> ```TS:Nada
> function FormatC(format : String, p1 : T, p2 : T, p3 : T, p4 : T, p5 : T, p6 : T, p7 : T, p8 : T, p9 : T, p10 : T) : String
> ``` 


---  
 #  FromRune : [string](string.md)

 `static`

> Constructs a string from the utf-8 code point of a rune.
> |Name|Type|Description|
> |---|---|---|
> |p0|[integer](integer.md)| |
> ```TS:Nada
> function FromRune(p0 : Integer) : String
> ``` 


---  
 #  FromRune : [string](string.md)

 `static`

> Constructs a string from a rune.
> |Name|Type|Description|
> |---|---|---|
> |p0|[rune](rune.md)| |
> ```TS:Nada
> function FromRune(p0 : Rune) : String
> ``` 


---  
 #  Get : [rune](rune.md)

> String operator Get is deprecated. To iterate through a String use a StringRange (.All) or StringIterator (.Begin).
> |Name|Type|Description|
> |---|---|---|
> |index|[integer](integer.md)| |
> ```TS:Nada
> function Get(index : Integer) : Rune
> ``` 


---  
 #  IsNullOrEmpty : [boolean](boolean.md)

 `static`

> Returns if the given string is null or empty.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function IsNullOrEmpty(p0 : StringRange) : Boolean
> ``` 


---  
 #  IsNullOrWhitespace : [boolean](boolean.md)

 `static`

> Returns if the given string is null, empty, or all whitespace.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function IsNullOrWhitespace(p0 : StringRange) : Boolean
> ``` 


---  
 #  Join : [string](string.md)

 `static`

> Concatenates the given strings with the given separator string.
> |Name|Type|Description|
> |---|---|---|
> |separator|[stringrange](stringrange.md)| |
> |value0|[stringrange](stringrange.md)| |
> |value1|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Join(separator : StringRange, value0 : StringRange, value1 : StringRange) : String
> ``` 


---  
 #  Join : [string](string.md)

 `static`

> Concatenates the given strings with the given separator string.
> |Name|Type|Description|
> |---|---|---|
> |separator|[stringrange](stringrange.md)| |
> |value0|[stringrange](stringrange.md)| |
> |value1|[stringrange](stringrange.md)| |
> |value2|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Join(separator : StringRange, value0 : StringRange, value1 : StringRange, value2 : StringRange) : String
> ``` 


---  
 #  Join : [string](string.md)

 `static`

> Concatenates the given strings with the given separator string.
> |Name|Type|Description|
> |---|---|---|
> |separator|[stringrange](stringrange.md)| |
> |value0|[stringrange](stringrange.md)| |
> |value1|[stringrange](stringrange.md)| |
> |value2|[stringrange](stringrange.md)| |
> |value3|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Join(separator : StringRange, value0 : StringRange, value1 : StringRange, value2 : StringRange, value3 : StringRange) : String
> ``` 


---  
 #  Replace : [string](string.md)

> Returns a new string with all occurances of a substrings replaced with another substring.
> |Name|Type|Description|
> |---|---|---|
> |oldValue|[stringrange](stringrange.md)| |
> |newValue|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Replace(oldValue : StringRange, newValue : StringRange) : String
> ``` 


---  
 #  RuneIteratorFromByteIndex : [runeiterator](runeiterator.md)

> Finds the iterator from a byte index. WARNING: Strings are UTF8 and constructing an iterator from bytes indices can make an iterator in the middle of a rune.
> |Name|Type|Description|
> |---|---|---|
> |byteIndex|[integer](integer.md)| |
> ```TS:Nada
> function RuneIteratorFromByteIndex(byteIndex : Integer) : RuneIterator
> ``` 


---  
 #  RuneIteratorFromRuneIndex : [runeiterator](runeiterator.md)

> Finds the iterator from a rune index. WARNING: this may be slow as finding an iterator from rune index requires a linear search.
> |Name|Type|Description|
> |---|---|---|
> |runeIndex|[integer](integer.md)| |
> ```TS:Nada
> function RuneIteratorFromRuneIndex(runeIndex : Integer) : RuneIterator
> ``` 


---  
 #  Split : [stringsplitrange](stringsplitrange.md)

> Splits the string, according to the separator string, into a range of substrings.
> |Name|Type|Description|
> |---|---|---|
> |separator|[stringrange](stringrange.md)| |
> ```TS:Nada
> function Split(separator : StringRange) : StringSplitRange
> ``` 


---  
 #  StartsWith : [boolean](boolean.md)

> Returns if the string starts with the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ```TS:Nada
> function StartsWith(p0 : StringRange) : Boolean
> ``` 


---  
 #  SubString : [string](string.md)

> 
> |Name|Type|Description|
> |---|---|---|
> |start|[runeiterator](runeiterator.md)| |
> |end|[runeiterator](runeiterator.md)| |
> ```TS:Nada
> function SubString(start : RuneIterator, end : RuneIterator) : String
> ``` 


---  
 #  SubStringBytes : [stringrange](stringrange.md)

> Constructs a substring based upon a number of bytes. WARNING: strings are UTF8 so indexing by bytes could produce unexpected results on non-ascii strings.
> |Name|Type|Description|
> |---|---|---|
> |startByteIndex|[integer](integer.md)| |
> |lengthInBytes|[integer](integer.md)| |
> ```TS:Nada
> function SubStringBytes(startByteIndex : Integer, lengthInBytes : Integer) : StringRange
> ``` 


---  
 #  SubStringFromRuneIndices : [string](string.md)

> Creates a substring from start and end indices. WARNING: this may be slow as finding an index for a UTF8 string requires a linear search.
> |Name|Type|Description|
> |---|---|---|
> |startIndex|[integer](integer.md)| |
> |endIndex|[integer](integer.md)| |
> ```TS:Nada
> function SubStringFromRuneIndices(startIndex : Integer, endIndex : Integer) : String
> ``` 


---  
 #  ToLower : [string](string.md)

> Returns a copy of the string that has been converted to lowercase.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ToLower() : String
> ``` 


---  
 #  ToUpper : [string](string.md)

> Returns a copy of the string that has been converted to uppercase.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function ToUpper() : String
> ``` 


---  
 #  Trim : [stringrange](stringrange.md)

> Trims all leading and trailing whitespace.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function Trim() : StringRange
> ``` 


---  
 #  TrimEnd : [stringrange](stringrange.md)

> Trims all trailing whitespace.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TrimEnd() : StringRange
> ``` 


---  
 #  TrimStart : [stringrange](stringrange.md)

> Trims all leading whitespace.
> |Name|Type|Description|
> |---|---|---|
> ```TS:Nada
> function TrimStart() : StringRange
> ``` 


---  
 

 
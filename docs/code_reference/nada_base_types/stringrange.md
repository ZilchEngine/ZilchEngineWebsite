 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[ Compare](stringrange.md#compare-zilch-engine-docu)|[ All](stringrange.md#all-zilch-engine-document)| | |
|[ CompareTo](stringrange.md#compareto-zilch-engine-do)|[ Begin](stringrange.md#begin-zilch-engine-docume)| | |
|[ Contains](stringrange.md#contains-zilch-engine-doc)|[ Current](stringrange.md#current-zilch-engine-docu)| | |
|[ EndsWith](stringrange.md#endswith-zilch-engine-doc)|[ Empty](stringrange.md#empty-zilch-engine-docume)| | |
|[ FindFirstOf](stringrange.md#findfirstof-zilch-engine)|[ End](stringrange.md#end-zilch-engine-document)| | |
|[ FindLastOf](stringrange.md#findlastof-zilch-engine-d)|[ IsNotEmpty](stringrange.md#isnotempty-zilch-engine-d)| | |
|[ FindRangeExclusive](stringrange.md#findrangeexclusive-zero)|[ OriginalString](stringrange.md#originalstring-zilch-engi)| | |
|[ FindRangeInclusive](stringrange.md#findrangeinclusive-zero)| | | |
|[ MoveNext](stringrange.md#movenext-void)| | | |
|[ Replace](stringrange.md#replace-zilch-engine-docu)| | | |
|[ RuneIteratorFromByteIndex](stringrange.md#runeiteratorfrombyteinde)| | | |
|[ RuneIteratorFromRuneIndex](stringrange.md#runeiteratorfromruneinde)| | | |
|[ Split](stringrange.md#split-zilch-engine-docume)| | | |
|[ StartsWith](stringrange.md#startswith-zilch-engine-d)| | | |
|[ Constructor](stringrange.md#stringrange-void)| | | |
|[ SubString](stringrange.md#substring-zilch-engine-do)| | | |
|[ SubStringBytes](stringrange.md#substringbytes-zilch-engi)| | | |
|[ ToLower](stringrange.md#tolower-zilch-engine-docu)| | | |
|[ ToString](stringrange.md#tostring-zilch-engine-doc)| | | |
|[ ToUpper](stringrange.md#toupper-zilch-engine-docu)| | | |
|[ Trim](stringrange.md#trim-zilch-engine-documen)| | | |
|[ TrimEnd](stringrange.md#trimend-zilch-engine-docu)| | | |
|[ TrimStart](stringrange.md#trimstart-zilch-engine-do)| | | |


 #  Properties


---  
 #  All : [stringrange](stringrange.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var All : StringRange


---  
 #  Begin : [runeiterator](runeiterator.md)

 `read-only`

> Returns the RuneIterator at the start of this range.
> ``` lang=cpp, name=Nada
> var Begin : RuneIterator


---  
 #  Current : [rune](rune.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Current : Rune


---  
 #  Empty : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var Empty : Boolean


---  
 #  End : [runeiterator](runeiterator.md)

 `read-only`

> Returns the RuneIterator at the end (one past the last Rune) of this range.
> ``` lang=cpp, name=Nada
> var End : RuneIterator


---  
 #  IsNotEmpty : [boolean](boolean.md)

 `read-only`

> 
> ``` lang=cpp, name=Nada
> var IsNotEmpty : Boolean


---  
 #  OriginalString : [string](string.md)

 `read-only`

> Returns the entire string that this range was constructed from.
> ``` lang=cpp, name=Nada
> var OriginalString : String


---  
 #  Methods


---  
 #  Compare : [integer](integer.md)

 `static`

> Compares the two string ranges and returns an integer to denote their relative sort order.
> |Name|Type|Description|
> |---|---|---|
> |left|[stringrange](stringrange.md)| |
> |right|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Compare(left : StringRange, right : StringRange) : Integer
> ``` 


---  
 #  CompareTo : [integer](integer.md)

> Returns if this string range is equal to the given range.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function CompareTo(p0 : StringRange) : Integer
> ``` 


---  
 #  Contains : [boolean](boolean.md)

> Returns if the string Contains the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Contains(p0 : StringRange) : Boolean
> ``` 


---  
 #  EndsWith : [boolean](boolean.md)

> Returns if the string ends with the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function EndsWith(p0 : StringRange) : Boolean
> ``` 


---  
 #  FindFirstOf : [stringrange](stringrange.md)

> Returns a StringRange that Contains the first occurrence of given StringRange.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function FindFirstOf(p0 : StringRange) : StringRange
> ``` 


---  
 #  FindLastOf : [stringrange](stringrange.md)

> Returns a StringRange that Contains the last occurrence of given StringRange.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function FindLastOf(p0 : StringRange) : StringRange
> ``` 


---  
 #  FindRangeExclusive : [stringrange](stringrange.md)

> Finds the first StringRange that starts with 'startRange' and ends with 'endRange'. This substring excludes 'startRange' and 'endRange'.
> |Name|Type|Description|
> |---|---|---|
> |startRange|[stringrange](stringrange.md)| |
> |endRange|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function FindRangeExclusive(startRange : StringRange, endRange : StringRange) : StringRange
> ``` 


---  
 #  FindRangeInclusive : [stringrange](stringrange.md)

> Finds the first StringRange that starts with 'startRange' and ends with 'endRange'. This substring includes 'startRange' and 'endRange'.
> |Name|Type|Description|
> |---|---|---|
> |startRange|[stringrange](stringrange.md)| |
> |endRange|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function FindRangeInclusive(startRange : StringRange, endRange : StringRange) : StringRange
> ``` 


---  
 #  MoveNext : Void

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function MoveNext()
> ``` 


---  
 #  Replace : [string](string.md)

> Returns a new string with all occurances of a substrings replaced with another substring.
> |Name|Type|Description|
> |---|---|---|
> |oldValue|[stringrange](stringrange.md)| |
> |newValue|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Replace(oldValue : StringRange, newValue : StringRange) : String
> ``` 


---  
 #  RuneIteratorFromByteIndex : [runeiterator](runeiterator.md)

> Finds the iterator from a byte index. WARNING: Strings are UTF8 and constructing an iterator from bytes indices can make an iterator in the middle of a rune.
> |Name|Type|Description|
> |---|---|---|
> |byteIndex|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function RuneIteratorFromByteIndex(byteIndex : Integer) : RuneIterator
> ``` 


---  
 #  RuneIteratorFromRuneIndex : [runeiterator](runeiterator.md)

> Finds the iterator from a rune index (the 'character' index). WARNING: this may be slow as finding an iterator from rune index requires a linear search.
> |Name|Type|Description|
> |---|---|---|
> |runeIndex|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function RuneIteratorFromRuneIndex(runeIndex : Integer) : RuneIterator
> ``` 


---  
 #  Split : [stringsplitrange](stringsplitrange.md)

> Splits the string, according to the separator string, into a range of substrings.
> |Name|Type|Description|
> |---|---|---|
> |separator|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function Split(separator : StringRange) : StringSplitRange
> ``` 


---  
 #  StartsWith : [boolean](boolean.md)

> Returns if the string ends with the specified substring.
> |Name|Type|Description|
> |---|---|---|
> |p0|[stringrange](stringrange.md)| |
> ``` lang=cpp, name=Nada
> function StartsWith(p0 : StringRange) : Boolean
> ``` 


---  
 #  StringRange : Void

 `constructor`

> 
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function StringRange()
> ``` 


---  
 #  SubString : [stringrange](stringrange.md)

> Constructs a StringRange from the given begin and end iterators.
> |Name|Type|Description|
> |---|---|---|
> |begin|[runeiterator](runeiterator.md)| |
> |end|[runeiterator](runeiterator.md)| |
> ``` lang=cpp, name=Nada
> function SubString(begin : RuneIterator, end : RuneIterator) : StringRange
> ``` 


---  
 #  SubStringBytes : [stringrange](stringrange.md)

> Constructs a substring based upon a number of bytes. WARNING: strings are UTF8 so indexing by bytes could produce unexpected results on non-ascii strings.
> |Name|Type|Description|
> |---|---|---|
> |startByteIndex|[integer](integer.md)| |
> |lengthInBytes|[integer](integer.md)| |
> ``` lang=cpp, name=Nada
> function SubStringBytes(startByteIndex : Integer, lengthInBytes : Integer) : StringRange
> ``` 


---  
 #  ToLower : [string](string.md)

> Returns a copy of the string that has been converted to lowercase.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToLower() : String
> ``` 


---  
 #  ToString : [string](string.md)

> Returns a new string of the current range.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToString() : String
> ``` 


---  
 #  ToUpper : [string](string.md)

> Returns a copy of the string that has been converted to uppercase.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function ToUpper() : String
> ``` 


---  
 #  Trim : [stringrange](stringrange.md)

> Trims all leading and trailing whitespace.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function Trim() : StringRange
> ``` 


---  
 #  TrimEnd : [stringrange](stringrange.md)

> Trims all trailing whitespace.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function TrimEnd() : StringRange
> ``` 


---  
 #  TrimStart : [stringrange](stringrange.md)

> Trims all leading whitespace.
> |Name|Type|Description|
> |---|---|---|
> ``` lang=cpp, name=Nada
> function TrimStart() : StringRange
> ``` 


---  
 

 
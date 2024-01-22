 `Core`

|Methods|Properties|Base Classes|Derived Classes|
|---|---|---|---|
|[AddTrailingDirectorySeparator](filepath.md#addtrailingdirectorysepa)|[DirectorySeparator](filepath.md#directoryseparator-zero)| | |
|[ChangeExtension](filepath.md#changeextension-zilch-eng)|[ExecutableDirectory](filepath.md#executabledirectory-zero)| | |
|[CombineDirectories](filepath.md#combinedirectories-zero)|[ExecutableFile](filepath.md#executablefile-zilch-engi)| | |
|[CombineDirectoriesAndFile](filepath.md#combinedirectoriesandfil)|[TemporaryDirectory](filepath.md#temporarydirectory-zero)| | |
|[GetCanonicalizedPathFromAbsolutePath](filepath.md#getcanonicalizedpathfrom)|[UserDocumentsDirectory](filepath.md#userdocumentsdirectory-z)| | |
|[GetComparablePathFromAbsolutePath](filepath.md#getcomparablepathfromabs)|[UserLocalDirectory](filepath.md#userlocaldirectory-zero)| | |
|[GetDirectoryName](filepath.md#getdirectoryname-zilch-en)|[WorkingDirectory](filepath.md#workingdirectory-zilch-en)| | |
|[GetDirectoryPath](filepath.md#getdirectorypath-zilch-en)| | | |
|[GetExtensionWithDot](filepath.md#getextensionwithdot-zero)| | | |
|[GetExtensionWithoutDot](filepath.md#getextensionwithoutdot-z)| | | |
|[GetFileNameWithExtension](filepath.md#getfilenamewithextension)| | | |
|[GetFileNameWithoutExtension](filepath.md#getfilenamewithoutextens)| | | |
|[IsRelative](filepath.md#isrelative-zilch-engine-d)| | | |
|[RemoveTrailingDirectorySeparator](filepath.md#removetrailingdirectorys)| | | |


 #  Properties


---  
 #  DirectorySeparator : [string](string.md)

 `read-only` `static`

> Gets the character(s) used for separating directories and files. This value is often different depending on the operating system (generally either '/' or '\')

> ```TS:Nada
> var DirectorySeparator : String


---  
 #  ExecutableDirectory : [string](string.md)

 `read-only` `static`

> The directory the executable lives with in (exe, elf...). This will always include a directory separator at the end of the result.

> ```TS:Nada
> var ExecutableDirectory : String


---  
 #  ExecutableFile : [string](string.md)

 `read-only` `static`

> A path directly to the executable itself (exe, elf...).

> ```TS:Nada
> var ExecutableFile : String


---  
 #  TemporaryDirectory : [string](string.md)

 `read-only` `static`

> Temporary files should be placed here. This will always include a directory separator at the end of the result.

> ```TS:Nada
> var TemporaryDirectory : String


---  
 #  UserDocumentsDirectory : [string](string.md)

 `read-only` `static`

> User saved data that the user can backup or modify should be placed here (read/write/create permissions should be allowed). This will always include a directory separator at the end of the result.

> ```TS:Nada
> var UserDocumentsDirectory : String


---  
 #  UserLocalDirectory : [string](string.md)

 `read-only` `static`

> Application saved information should be placed here (read/write/create permissions should be allowed). This will always include a directory separator at the end of the result.

> ```TS:Nada
> var UserLocalDirectory : String


---  
 #  WorkingDirectory : [string](string.md)

 `static`

> A directory that all relative paths start resolving from. In general the changing of the working directory is discouraged because it may affect assumptions of the host application. This will always include a directory separator at the end of the result.

> ```TS:Nada
> var WorkingDirectory : String


---  
 #  Methods


---  
 #  AddTrailingDirectorySeparator : [string](string.md)

 `static`

> Pass in a directory path with or without the separator and this will add it at the end (if needed).
Example: ('Content\Powerups') results in 'Content\Powerups\'
Example: ('Content\Powerups\') results in 'Content\Powerups\'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function AddTrailingDirectorySeparator(p0 : String) : String
> ``` 


---  
 #  ChangeExtension : [string](string.md)

 `static`

> Changes the extension of a path (with file name at the end) to a new extension. If the file has no extension, then this will automatically add the extension to the end. The extension is allowed to contain a leading dot '.' character (or not). The path is also allowed to contain a trailing dot '.' character (or not).
Example: ('Content\Player.png', 'jpg') results in 'Content\Player.jpg'
Example: ('Content\Player', 'jpg') results in 'Content\Player.jpg'
Example: ('Content\Player.', '.jpg') results in 'Content\Player.jpg'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> |p1|[string](string.md)| |
> ```TS:Nada
> function ChangeExtension(p0 : String, p1 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> ```TS:Nada
> function CombineDirectories(dir0 : String, dir1 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |dir2|[string](string.md)| |
> ```TS:Nada
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |dir2|[string](string.md)| |
> |dir3|[string](string.md)| |
> ```TS:Nada
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String, dir3 : String) : String
> ``` 


---  
 #  CombineDirectories : [string](string.md)

 `static`

> Combines directory paths and directories names together (empty entries are skipped). This will always include a directory separator at the end of the result.
Example: ('Content', 'Powerups') results in 'Content\Powerups\'
Example: ('Content\', 'Powerups\') results in 'Content\Powerups\'
Example: ('Content\', '', 'Powerups') results in 'Content\Powerups\'
Example: ('C:\Sandbox\', 'Content') results in 'C:\Sandbox\Content\'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |dir2|[string](string.md)| |
> |dir3|[string](string.md)| |
> |dir4|[string](string.md)| |
> ```TS:Nada
> function CombineDirectories(dir0 : String, dir1 : String, dir2 : String, dir3 : String, dir4 : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |fileName|[string](string.md)| |
> ```TS:Nada
> function CombineDirectoriesAndFile(dir0 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |fileName|[string](string.md)| |
> ```TS:Nada
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |dir2|[string](string.md)| |
> |fileName|[string](string.md)| |
> ```TS:Nada
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, dir2 : String, fileName : String) : String
> ``` 


---  
 #  CombineDirectoriesAndFile : [string](string.md)

 `static`

> Combines directory paths, directories names, and a single file name together (empty entries are skipped). Because we are combining a file name at the end, this will not result in a trailing directory separator.
Example: ('Content\Powerups\', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content\Powerups', '', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('Content', 'Powerups', 'Recharge.png') results in 'Content\Powerups\Recharge.png'
Example: ('C:\Sandbox\', 'Content\Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |dir0|[string](string.md)| |
> |dir1|[string](string.md)| |
> |dir2|[string](string.md)| |
> |dir3|[string](string.md)| |
> |fileName|[string](string.md)| |
> ```TS:Nada
> function CombineDirectoriesAndFile(dir0 : String, dir1 : String, dir2 : String, dir3 : String, fileName : String) : String
> ``` 


---  
 #  GetCanonicalizedPathFromAbsolutePath : [string](string.md)

 `static`

> Changes all directory separators to be the current operating system directory separator, removes duplicate separators, and removes '..' and '.' from the paths. Canonicalized is only guaranteed to work on absolute paths. This behavior is operating system dependent and may call the related OS functions.
Example: ('C:/Sandbox//Engine/../Content/./Player.png') results in 'C:\Sandbox\Content\Player.png'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetCanonicalizedPathFromAbsolutePath(p0 : String) : String
> ``` 


---  
 #  GetComparablePathFromAbsolutePath : [string](string.md)

 `static`

> First this normalizes the path, then if the operating system is case insensative, it will make the path all lowercase so that it compares.
Example: ('C:\Sandbox\Engine\..\Content\.\Player.png') results in 'c:\sandbox\content\player.png'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetComparablePathFromAbsolutePath(p0 : String) : String
> ``` 


---  
 #  GetDirectoryName : [string](string.md)

 `static`

> If a file path is passed in, this will return the name of the parent directory. If a directory path is passed in (ending in a separator), this will return the name of the directory. A directory path without a trailing separator is abiguous with a file that has no extension. In this case, we always assume it is a file and therefore get the parent directory's name.
Example: ('Content\Powerups\Recharge.png') results in 'Powerups'
Example: ('Content\Powerups\') results in 'Powerups'
Example: ('Content\Powerups') results in 'Content'
Example: ('Content') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetDirectoryName(p0 : String) : String
> ``` 


---  
 #  GetDirectoryPath : [string](string.md)

 `static`

> If a file path is passed in, this will return the parent directory. If a directory path is passed in (ending in a separator), this will return the directy back with no modifications. A directory path without a trailing separator is abiguous with a file that has no extension. This will always include a directory separator at the end of the result. In this case, we always assume it is a file and therefore get the parent directory's name.
Example: ('Content\Powerups\Recharge.png') results in 'Content\Powerups\'
Example: ('Content\Powerups\') results in 'Content\Powerups\'
Example: ('Content\Powerups') results in 'Content\'
Example: ('Content') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetDirectoryPath(p0 : String) : String
> ``` 


---  
 #  GetExtensionWithDot : [string](string.md)

 `static`

> Returns only the extension of a file (everything after the last dot, including the dot). If the file has no extension then this will return an empty string.
Example: ('Content\Player.png') results in '.png'
Example: ('Content\Player.') results in ''
Example: ('Parent.Directory\Log') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetExtensionWithDot(p0 : String) : String
> ``` 


---  
 #  GetExtensionWithoutDot : [string](string.md)

 `static`

> Returns only the extension of a file (everything after the last dot, not including the dot). If the file has no extension then this will return an empty string.
Example: ('Content\Player.png') results in 'png'
Example: ('Content\Player.') results in ''
Example: ('Parent.Directory\Log') results in ''

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetExtensionWithoutDot(p0 : String) : String
> ``` 


---  
 #  GetFileNameWithExtension : [string](string.md)

 `static`

> Returns only the file portion of a path (everything past the last separator including the extension).
Example: ('Content\Player.png') results in 'Player.png'
Example: ('Content\Powerups\') results in ''
Example: ('Content\Powerups') results in 'Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetFileNameWithExtension(p0 : String) : String
> ``` 


---  
 #  GetFileNameWithoutExtension : [string](string.md)

 `static`

> Returns only the file portion of a path (everything past the last separator excluding the extension).
Example: ('Content\Player.png') results in 'Player'
Example: ('Content\Powerups\') results in ''
Example: ('Content\Powerups') results in 'Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function GetFileNameWithoutExtension(p0 : String) : String
> ``` 


---  
 #  IsRelative : [boolean](boolean.md)

 `static`

> Returns true if a path has no root (such as a volume/hard drive specifier, or unix like systems a beginning slash). Even a beginning slash that means 'relative to the current working directory volume' is still relative. Empty paths will return that they are relative.
Example: ('C:\Sandbox\Engine\..\Content\.\Player.png') results in 'false'
Example: ('Sandbox') results in 'true'
Example: ('Content\Powerups\Recharge.png') results in 'true'
Example: ('/usr/Content/Player.png') results in 'false'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function IsRelative(p0 : String) : Boolean
> ``` 


---  
 #  RemoveTrailingDirectorySeparator : [string](string.md)

 `static`

> Pass in a directory path with or without the separator and this will remove it from the end (if needed).
Example: ('Content\Powerups') results in 'Content\Powerups'
Example: ('Content\Powerups\') results in 'Content\Powerups'

> |Name|Type|Description|
> |---|---|---|
> |p0|[string](string.md)| |
> ```TS:Nada
> function RemoveTrailingDirectorySeparator(p0 : String) : String
> ``` 


---  
 

 
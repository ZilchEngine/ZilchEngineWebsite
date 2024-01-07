This page covers how to export your project.

 # Export to a stand alone executable
For small projects this is the easiest option. It will produce an executable that should run on any windows machine

 - Open your project
 - Run the [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands.md) : [ExportGame](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#exportgame)
 - Select a executable file name
 - You are done!

 # Export for an installer
If you project is a very large stand alone, executable may not be the right options since it has to extract the files when it runs.

 - Open your project
 - Run the [Command](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/editor/editorcommands.md) : [ExportContent](https://github.com/ZilchEngine/ZilchDocs/blob/master/code_reference/command_reference.md#exportcontent)
 - A folder will be opened will all the files that need to be in the installer
 - The [Inno-Setup ](http://www.jrsoftware.org/isdl.php ) file will generate an installer
   ![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47333.png)
 

 
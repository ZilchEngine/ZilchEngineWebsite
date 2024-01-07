This explains what and how tags are used in the Zilch Engine. 

 # Conceptually
Tags are an alternate form of organization to the hierarchical folders.
Properties of Tags:

 - Tags represent ideas or categories that are associated with an object.
 - Multiple tags can be associated with a single object. 
 - Objects are found by filtering all available objects by their tags, thus each object would at least need one tag to be found. 
 - Each additional tag used while searching would further restrict the results; however, the order in which the filtering is applied would not change the **final** result. Thus, 



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47337.png)


would show the same objects as 



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47339.png)


and



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47341.png)


and all other permutations of tags.

 # Tags in Zilch
Tags in the Zilch Engine are used in the Library Window to organize the [Resources](https://github.com/ZilchEngine/ZilchDocs/blob/master/zilch_editor_documentation/zilchmanual/architecture/resources/resources.md). 

 ## Adding and Removing Tags
Right-clicking on an object in the `Library Window` will give you the option to Edit Tags:



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47343.png)


Here you can add tags 



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47345.png)


and remove them using the x button. 



![image](https://raw.githubusercontent.com/ZilchEngine/ZilchFiles/master/doc_files/47347.png)


 ## Automatically Generated Tags
There are a few automatically generated tags, such as Archetype , Level , Texture , etc. These arise from the need to have a tag for every object so that they can show up when you search. They are added when you add the resource and cannot be removed. This prevents a user from losing the ability to access a resource they created.
 

 
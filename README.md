# Presentation
<h1>Goals and Objectives</h1>

1) To create a database schema of images obtained by capturing stills of 3d objects in different angles along X, Y and Z axis by using Maya Software.<br>
2) The main objective of this database schema is to use it for training the Capsule Network which is used in identification of 3D object s in real world.<br>
3) To build the structure of database schema  in such a way that user should be able to extract data according to any parameter that he wants to in terms of resolution, size, texture and angles and other parameters.<br>

<h1>Problems to be Addressed</h1><br>
1-In the sectors of military areas and borders, it is important to know the weapons, ammunations being carried by the enemy. By understanding these weapons, one can figure out particular strategies or risk to be implemented. Here, the dataset of weapons can be used for training purpose<br>
2-Cancer and tumors is another important problem which is being addressed with the help of Capsule Neural Networks. Here, CNN can be used for early detection of cancer and tumor.<br>
3-In environmental areas like water and solid waste, CNN can be implemented in detection and segregation of waste materials.<br>

<h1>Potential pitfalls and challenges</h1>
We are not generating 360 view of the object as there is no bottom view of the object.
The system will be difficult to predict or translate monuments in very bright light conditions or in extremely dark environments.

<h1>Resources</h1>
To accomplish our task we have used several resources like Maya Software for generating the images.
We have also used softwares like Blender and Autodesk 3ds MAX. These softwares were used to convert the object from type max and blend to type obj.



<h1>Background Research</h1>

Inorder to create a database of images, first of all we tried scrapping the properties of single image in a folder using the following code:<br>


![Pythoncode](https://user-images.githubusercontent.com/46699516/56156629-a253bb00-5f8b-11e9-8218-a8f57518e614.PNG)

Then according to the following Database Schema, tried scrapping the image properties like path, size, resolution and type.

![Images_ERDiagram](https://user-images.githubusercontent.com/46699516/56158182-615da580-5f8f-11e9-823a-7c2d9ed1b6c1.png)

In the above database schema,tables sub_object and category_object are not in 2NF, hence inorder to satisfy it we have to break the two tables and below is the updated ER Diagram for the same



Python code to get the properties of the images given the root directory, we can get all the subfolder and the files present in it.

![ImageProperties1](https://user-images.githubusercontent.com/46699516/56158220-7b978380-5f8f-11e9-8335-e153351aedd8.PNG)

![ImageProperties2](https://user-images.githubusercontent.com/46699516/56158280-9e299c80-5f8f-11e9-85ad-dcaa17f53806.PNG)



<h1>Next Steps to be taken</h1>

We intend to create a website which will act as a platform from where we can have multiple use case on the image database that we created<br>
From the website we can store all the user and image related information and then following can be our use cases.

<h1>Use Cases</h1>
1)List of users who have downloaded a particular image<br>
2)Which image is downloaded the most<br>
3)Images with resolution greater than 1000*500<br>
4)List of Images of a given category<br>
5)Images with size greater than the given size<br>
6)list of Users selecting images of a given category<br>

<h1>References</h1>
https://stackoverflow.com<br>
www.autodesk.com<br>


<h1>License</h1>
MIT License<br>

Copyright (c) 2019 Rashika Moza, Akash Srivastava and Aditya<br>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:<br>

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.<br>

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# OpenGL_Learning
In this project we are going to learn few basics of legacy and modern openGL.

We have used GLFW library for windowing.In other words all this library is going to do is provide us with the appropriate platform layer i.e., it is going to provide us with an implementation of that windowing creation code and management code as well for Windows,Mac and Linux.

We also used GLEW library in this project.Since we have developed this project in Windows,and and their kind of OpenGL implementation goes only till OpenGL 1.1 and since we need to use modern OpenGL too so in our system we need a way to actually get all of the modern OpenGL functions.OpenGL functions are implemented in our GPU drivers.So,we need to get into those drivers,pull out the functions and call them.We need to access the drivers' DLL files and just retrieve function pointers to the functions inside those libraries that's what we need to do.So,we can do this manually or we can use another lirary.So,what this library actually does is it provides the OpenGL API specification kind of function declarartions and symbol declarartions and constatnts and all that stuff for us in a header file and then kind of the behind scenes file(the CPP file in our case) the actual implementation pf the library goes into our IDE,it identifies what graphics drivers we are using,finds the appropriate DLL file and then loads all the function pointers thats what it does,thats what it all does.This library doesn't implement the functions or anything,they don't they just access the functions that are already on our computer in binary form and library that we are going to use that does that for us is something called GLEW(OpenGL extension wrangler),other is GLAD.




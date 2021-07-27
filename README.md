# Simple Raycaster
A simple raycaster implemented in C and OpenGL

## Ray Casting
Ray casting is capable of transforming a limited form of data into a three-dimensional projection with the help of tracing rays from the view point into the viewing volume. The main principle behind ray casting is that rays can be cast and traced in groups based on certain geometric constraints. In ray casting, a ray from the pixel through the camera is obtained and the intersection of all objects in the picture is computed. Next, the pixel value from the closest intersection is obtained and is further set as the base for the projection. Ray casting is distinct from ray tracing, with ray casting being a rendering algorithm which would never recursively trace secondary rays, while ray tracing is capable of doing so. Ray casting is also simple to use compared to other rendering algorithms such as ray tracing.

Ray casting is fast, as only a single computation is needed for every vertical line of the screen. Compared to ray tracing, ray casting is faster, as it is limited by one or more geometric constraints. This is one of the reasons why ray casting was the most popular rendering tool in early 3-D video games.

However compared to ray tracing, the images generated with ray casting are not very realistic. Due to the geometric constraints involved in the process, not all shapes can be rendered by ray casting. You can learn more from [here](https://people.cs.clemson.edu/~dhouse/courses/405/notes/raycast.pdf).

## Dependencies and Softwares
* `GLUT` : OpenGL Utility Toolkit, a window system independent toolkit for writing OpenGL programs. You can get the GLUT libraries and dlls from [here](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbkpNcHFGbHJHRk5PYmg2Zll5eGRuM3U2VVlXZ3xBQ3Jtc0trUld2bE9PNlFfb1Z5RjBsY0hCaWxxRGNueEg0aXhNOVJnd0FSdkRKM2hETlRsYXFpck5wbnpfODdYenpBT3hTVmhiYUEwX3NFY0twajlHeDduMk5UNFhJaEczZUtoVVI4U0dBNFRiam45M3pvd2M2Yw&q=http%3A%2F%2Fchortle.ccsu.edu%2FBloodshed%2Fglutming.zip). You have to manually add the libraries and header files in your respective compiler location and add the dll in the system path.

* Dev-C++ : Dev-C++ is recommended for compilation as the program utilizes [MingW 4.7.2](http://mingw-w64.org/doku.php/versions#v4), which is quite old. You can download Dev-C++ from [here](http://www.mediafire.com/download/jvca73gqgg0l783/Setup_DEVC%2B%2B+5.4.1.rar).
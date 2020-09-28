---
layout: post
title: Compling OpenCV on Windows with MingW
---
For anyone interested, here is the process I used to successfully build OpenCV 2.4.8 with MingW on Windows 8 (64 bit) and setup Eclipse for development.

- Download MingW 32-bit from [MingW Website](http://www.mingw.org/) or [MingW SourceForge Repository](http://mingwrep.sourceforge.net/)
- Download OpenCV from [OpenCV Website](http://opencv.org/downloads.html) (Windows version).
- Download CMake from [CMake Website](http://www.cmake.org/)
- Extract the downloaded files into their corresponding folders. Folder structure on my PC is as follows:
  - C:\opencv
  - C:\cmake
  - C:\mingw
- Add C:\mingw\bin directory to system PATH
- Open CMake executable and select Source Code=C:/opencv/sources, and Destination=C:/opencv/mingw. Click on 'Configure' button and make sure that 'MingW Makefiles' option is selected. Click 'Configure' again and then click on the 'Generate' button.
- Open Windows command line and type 'cd C:/opencv/mingw', then type 'mingw32-make'. Once build process completes successfully, close the command line window.
- Open Eclipse and create a sample project (You can use following code to test):

> <code>#include &lt;opencv2/core/core.hpp&gt;<br>
> #include &lt;opencv2/highgui/highgui.hpp&gt;<br>
> #include &lt;opencv2/opencv.hpp&gt;<br>
> #include &lt;iostream><br>
>
> using namespace std;<br>
> using namespace cv;<br>
>
> int main()<br>
> {<br>
>
> Mat img = imread("c:/lenna.png", CV_LOAD_IMAGE_COLOR);<br>
>
> namedWindow("MyWindow", CV_WINDOW_AUTOSIZE);<br>
> imshow("MyWindow", img);<br>
>
> waitKey(0);<br>
> return 0;<br>
> }</code><br>

- Now, go to Project -> Properties -> C/C++ Build -> Settings -> MinGW C++ Linker -> Libraries, and add to the Libraries (-l) one by one, in Eclipse:
  - libopencv_calib3d248, libopencv_contrib248, libopencv_core248, libopencv_features2d248, libopencv_flann248 so and so on, depending on your code references.
  - Then add C:\opencv\mingw\lib under the Library search path (-L)
- Build the project and watch out for any errors in the Eclipse console.
Good Luck and Happy Coding!
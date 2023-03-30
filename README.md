# Binary Image Processor

## 1. Introduction 
Binary Image Processor program is written in pure python without using any external libraries except for NumPy and MatPlotLib for array manipulation and display of the image. This program allows various techniques of image processing to the input image. At present, the program only accepts grey-scaled image, that is, input file must end with PGM extension. 

Readme supplements the binaryImageProcessor.py as a manual. This manual only highlights a couple of operations as most of the operations in the program are self-explanatory.

## 1.1 How to run the program

Pre-requisite: 
•	Python Environment (Install Python if not already available in your computer: https://www.python.org/), 
•	NumPy and 
•	Matplotlib libraries. 

How-to-run:
1.	Download binaryImageProcessor.py 
2.	Open the terminal and locate to the directory of binaryImageProcessor.py 
3.	Run the program by typing: python3 binaryImageProcessor.py 
Note: At present, program only processes 1 image at one time. 

## 1.2  Simple Interface 
This is a scripting program. For simplicity sake, I do not convert our source code into an executable file. When run on the terminal, Program will introduce itself and ask the user to provide the file directory path of the image (recommended to keep the images in the same directory). Program only accepts PGM format file. Any other files are rejected. 
 
In the above interface, the user is asked to input the file name along with the ‘.pgm’ format used for the assignment. The user also has the liberty to provide the path to the image file.

### 1.2.1 Illustration for image input
 
 

### 1.2.2 Illustration for Image Processing Operations
Next, program displays a list of image processing operations, they are grouped by their category: Pre-processing and Edge Detection. User must enter the corresponding number to apply the operation to the input image. 
 
After choosing an option, program will perform the selected image processing technique to the image. Operation is not reversible and after each operation, the resulting image is display to the user. User has an option to continue apply the next operations or choose to quit. Resulting image is stored in the memory and a copy of resulting image is also saved to the same directory where the input image exists. 

User also has an option to load a new image, in which case, the resulting image in memory will be cleared and user will be starting with a fresh image. 

Illustration for Linear Stretching and Compression

For linear stretching and compression, user is asked to input the min pixel and max pixel values. From these two values and provided image’s min pixel and max pixel values, the slope is computed and display to the user. 

Note: 
Slope = 1 ==> Contrast unchanged
Slope > 1 ==> Stretching 
Slope < 1 ==> Compression


As such, the min and max values user can input are restrained to the image’s min and max pixel values. 

Example: min should be between 43 and 254. Max should be between min value and 255 for the slope to be < 1.
 

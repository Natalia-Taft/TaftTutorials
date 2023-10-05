# TaftTutorials
Tutorials for my lab and classes

# How to Load and Crop Large Files into Smaller Files in Slicer

## 1) Open Slicer
- Make sure you have the SlicerMorph module extension loaded

## 2) Go to Modules drop-down menu
![](FHLTTW_01)

<img src ="https://raw.githubusercontent.com/Natalia-Taft/TaftTutorials/main/TutorialImages/FHLTTW_01.png">

## 3) Drop down to SlicerMorph -> Input and Output -> ImageStacks
![](FHLTTW_02)

## 4) Choose your file
![](FHLTTW_03)
1) Open the "Input files" drop-down menu
1) Go to the hard drive (TaftNK_Storage)
2) Go to data folder (Sculpin Ray Project)
3) Select species (Myoxocephalus_scorpius)
4) Select Folder "OS_150220_TB25"
(Could take a while to load)
5) Scroll ALL the way down to the folder with the Reconstructed files (OS_150220_TB25_35.5um_2k_Rec)
6) Scroll down past the first twenty or so slices and click on any individual bmp file)
7) Click "Open"

## 5) Change the spacing of the input file to match your specific file
![](FHLTTW_04) 
1) Find the three Spacing boxes that read 1000mm
2) Change spacing from 1000mm to file-specific spacing To do this, convert the um in your file name to mm by dividing by 1000 (35.5 um -> .0355 mm for this file)
- *Note: The program often won't take the first zero right away, you may have to type .0355 and it will come out .355, and you have to go back and insert the first zero again so it will read .0355*
-  Make sure to copy and paste the correct spacing from the left box into the other two boxes
![](FHLTTW_05) 
![](FHLTTW_06) 

## 6) Preview Volume
1) Make sure that "preview" is clicked in the "Quality" menu
2) Check "output size"...should be megabytes, not gigabytes
3) Click "Load files" button
- *Note: Could take a few minutes*
(Insert image 6 here)

## 7) Visualize Preview in Volume Rendering
1) Go to the Modules drop-down menu and select the "Volume Rendering" Module
![](FHLTTW_07) 


## 8) Visualize your Preview
1) Click the "Eye" next to Volume so it is open
2) Click the "Center View" button, and re-size your volume so you can see it
3) In the Display menu, choose your Preset. We will almost always be using umCT-Bone8Bit
4) Adjust the Shift slider a TEENSY bit to make sure you can see the bones clearly, with minimal other stuff.
5) Click the eye icon next to "Display ROI" so that you can see your ROI in the 3D volume window as well as in the individual slice views
![](FHLTTW_08) 

## 10) Locate your region of interest and Crop
1) You can rotate your preview volume all around and locate the structure you are interested in, or use the slice views
2) Use the "dots" (black arrow in 3D view, blue arrow in Green window view) to re-size your ROI 
![](FHLTTW_09) 

## 11) Return to Image Stacks to Rename your new ROI
![](FHLTTW_10) 
Once you have your region of interest cropped, use the Module Drop-down menu to go to 
SlicerMorph -> Input and Output -> Image Stacks
1)  In the Output Volume, Create New Volume as...and rename your volume. 
2) Then, make sure your 'Region of Interest" is set to Volume rendering ROI
3) Change your Quality to "full resolution"
4) Check and make sure your file size is small (megabytes, not gigabytes)
5) Click "Load files"
*Note: This could take a few minutes*
![](FHLTTW_11) 

## 13) Check and Save
![](FHLTTW_12) 
1) After your file reloads at full resolution, time to check and save
2) If the new file looks good, go up and click the "Save Data" icon
3) Choose "Save Data", and it will giev you the option to choose where to save your data
4) Make sure you choose the right directory!
![](FHLTTW_13) 
5) This first time, save all of the files, the MRML Scene; the NNRD, the VolumeProperty and the Markups JSON files. 
Don't change the names of anything at this point! Just save!

Now you can come back and segment out your nice, smaller file!

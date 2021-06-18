# ETH-UCY-Preprocessing

------------------------------------------------------------------------------------------------------------------
Annotation files given in BIWI dataset (http://www.vision.ee.ethz.ch/en/datasets/) <br />
Info : Video frame rate: 2.5fps (6 frames = 0.04s)

------------------------------------------------------------------------------------------------------------------
Annotation files given in crowds dataset (https://graphics.cs.ucy.ac.cy/research/downloads/crowd-data) <br />
Info: Video frame rate: 25fps (1 frame = 0.04s). 

------------------------------------------------------------------------------------------------------------------

In this repository you will find the Python script and preprocessed data where: <br />

Data_Formated_<file name>.csv:      <br />   
Extracted data from (obsmat.txt for ETH data, .VSP file from the UCY dataset) and adjusted to the desired format which is [FrameID, PedID, PosX,PosY]  <br />  
(meters if its from the ETH dataset, and pixels if its from the UCY dataset)   
  
-------------------------------------------------------------------------------------------------------------------  

Data_in_meters_<file name>.csv:    <br />  
Data converted from image coordinates to world coordinates.  <br />                              
(meters)                                        
  
--------------------------------------------------------------------------------------------------------------------

interpolated_data_<file name>.csv:    <br />                           
Interpolate data from Data_in_meters for each frame. <br />
(meters)    
  
--------------------------------------------------------------------------------------------------------------------  

Final_data_<file name>.csv:    <br />        
Extract interpolated_data at every 10 frames (2.5fps)  <br />           
(meters)                                  

--------------------------------------------------------------------------------------------------------------------
UCY Preprocessing.ipynb,   ETH Preprocessing.ipynb: <br />
Python scripts for the preprocessing steps for each dataset.

--------------------------------------------------------------------------------------------------------------------
KNIME Analytics platform workflow:    <br />
A workflow for extracting data analytics and data cleaning.
  
--------------------------------------------------------------------------------------------------------------------

# MewRecorder
Video/Audio recorder for Telemed ultrasound machine. 

v1.0.4

Latest update: 07JUL2023

<p align="center"><img src="./Screenshots/MWR_main-screen.png" width="550"></p>

- "MewRecorder" is a MATLAB-based application for recording video and audio simultaneously on Telemed ultrasound machine (e.g., MicrUs Ext).
- It requires installation/running of EchoWave II software from Telemed.
- This app controls EchoWave to record ultrasound video and uses MATLAB to record audio.
------------------------------------------
### INSTALLATION
##### Requirements:
Current Telemed ultrasound machine only supports Windows PC. 
A faster PC running Windows 10 or 11 is recommended. 
Minimum system RAM requirements: > 16GB (64GB is preferred.) 
Needs to dedicate at least 5GB to EchoWave. 
(EchoWave -> Menu -> Customize -> Scanning Control -> Cine -> Cine Size:  Change this value to at least 5000 MB. The more the better but do not max out.)

- MATLAB:
-   R2022b or newer
-   Audio Toolbox

##### Steps:
1. Download all the files from this distribution and put them in a folder. 
2. Download a redistributed FFMPEG release in zip file from here and put it in the same folder (do not unzip):
   For Windows only: [ffmpeg.zip]([https://yaleedu-my.sharepoint.com/:u:/g/personal/wei-rong_chen_yale_edu/Ec0_HMhojDFCvtdyo0AjN8wBfkx9LccKPOwctLRuKnLWGQ?e=bB5M37]) 
------------------------------------------
### RUN
1. Run EchoWave II in Administraion first.
2. Run MATLAB. To control EchoWave, you must run MATLAB in Administration mode. 

- In MATLAB command window, type:
     >> cd ./MewRecorder  % [change this to your installation folder]  
     >> MewRecorder
     
### Alternative method (standalone app):
(MATLAB is not required)
You can download and install a standalone compiled app from here:
For Windows only: [MewRecorder_installer.zip]([https://yaleedu-my.sharepoint.com/:u:/g/personal/wei-rong_chen_yale_edu/EdBz8q17uFJOpks6ysuLr4IBz4YFsLuTm_21nVLe60RUnw?e=ZWGflK]) 
This installer includes all dependencies (e.g., ffmpeg). 
During installation, check "Add shortcut to desktop". 
After installation, right-click on the icon of MewRecorder and click "Run as administrator". 

### COPYRIGHT, LICENSE & DISCLAIMER
Copyright (C) 2020 Wei-Rong Chen <wei-rong.chen[AT]yale.edu>  
This program is free software under GNU General Public License, version 3.  
This program is distributed WITHOUT ANY FORM of EXPRESS or IMPLIED WARRANTY and ANY SUPPORT.    
See the GNU General Public License for more details.  




   
- The time-synchonization port should be connected to the second channel of the audio inputs. 

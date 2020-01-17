# newport_delay_stage_gui
## Description
This repository provides a GUI tool for controlling the [Newport delay line stage](https://www.newport.com/f/delay-line-stages). In order to control the stage, .NET Framework is used. This GUI works under the following condisionts:
- Windows 10
- Python3 (Anaconda)
- [DL Series Optical Delay Line Linear Motor Linear Translation Stages](https://www.newport.com/f/delay-line-stages)

## DLS_GUI_control
This tool consists of 2 files: DLS_GUI_control.py and myfunc.py. 

### Control Window
<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui.PNG" width="500px">  
  
If you run the DLS_GUI_control.py, a new window displayed above will show up. The window consists of 3 sections:
- CURRENT SETTINGS
- CHANGE SETTINGS
- DELAY SCAN

#### CURRENT SETTINGS
The section of the Current Settings shows the current values of the position, velocity, and acceleration. You can get the latest value by clicking the Update button. It is worth clicking several times when you move largely with very slow velocity.  

#### CHANGE SETTINGS
The Change Settings section allows you to change the position, velocity, and acceleration. You can type values and click the button placed right to the entry box. Move-to-x button initiates the movement of the stage to the target position. In order to check whether the stage has finished moving, you can click the Update button in the Current Settings section. Change-v and Change-a buttons allow us to change values and update the Current Settings section. If you want to change all values and update the Current Settings, you can click Change-x,v,and-a-at-once button. 

#### DELAY SCAN
This section allows you to do the automatic scan for several times. Once you specify the initial and final positions and number of steps, you can calculate scan step (s/step) and scan range (s) by clicking the Calculate-time-settings button.  
  
Once you start scanning, you can see the progress of the scan.

<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui_2.PNG" width="300px">

## myfunc
You can get the current position of your delay line stage.  

## Avoiding Expected Errors at the Beginning
- Please check whether you have [pythonnet](https://pypi.org/project/pythonnet/).
- Please check whether you are importing correct clr library.
- Please check the COM port.

## Useful References
- Official document: https://www.newport.com/mam/celum/celum_assets/resources/DL_Controller_-_Command_Interface_Manual.pdf?1
- My another repository: 

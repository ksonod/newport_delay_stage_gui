# newport_delay_stage_gui
GUI for controlling the Newport delay line stage




## Description
This repository contains simple python codes for controlling [Newport delay line stage](https://www.newport.com/f/delay-line-stages). You can start from here and modify them. In order to control the stage, .NET is used. These codes work under the following condisionts:
- Windows 10
- Python3 (Anaconda)
- [DL Series Optical Delay Line Linear Motor Linear Translation Stages](https://www.newport.com/f/delay-line-stages)

## DLS_GUI_control


<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui.PNG" width="500px">

<img src="https://github.com/ksonod/newport_delay_stage_gui/blob/master/dls_gui2.PNG" width="500px">

## myfunc
You can get the current position of your delay line stage.  

## Avoiding Expected Errors at the Beginning
- Please check whether you have [pythonnet](https://pypi.org/project/pythonnet/).
- Please check whether you are importing correct clr library.
- Please check the COM port.

## Useful References
- Official document: https://www.newport.com/mam/celum/celum_assets/resources/DL_Controller_-_Command_Interface_Manual.pdf?1
- My another repository: 

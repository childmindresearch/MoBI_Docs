# Tabletop Eye tracker: Lite by EyeLogic

<center>![eyelogic](img/EyeTracking_Tabletop/8.png)</center>

## Specifications


| _Specification_        | Details                                                                                                 |
|--------------------------|---------------------------------------------------------------------------------------------------------|
| _Sampling Rate_        | 60 Hz/120 Hz                                                                              |
| _Gaze Accuracy_        | < 0.50 (typical)                                                          |
| _Gaze Spatial Resolution_ | < 0.10 (typical)                                                                                        |
| _Operational Distance_         | 50 - 85 cm                                                                          |
| _Tracking Area_ | Width: 30 cm / height: 20 cm (@ 60 cm)                                                                            |
| _PC Interface_ | USB 3                                                                                                   |
| _Blink Recovery Time_          | 8 ms (@120 Hz)                                                                                       |
| _System Latency_ | 16 ms (@120 Hz)                                                            |
| _Screen Size_         | Up to 25 inch                                                                                     |
| _Technology_          | dark pupil, non-invasive video based                                                                                    |
| _Operating System_                  | Windows 10                                                                   |

## Hardware Setup

### Out of Box Setup for EyeLogic Eye Tracker

#### Equipment
The following equipment should be included in the Eyelogic Lite hardware: 

- Eye Tracker
- Metal Plates (to attach eye tracker to screen)
- Cleaning wipes

<center>![equipment](img/EyeTracking_Tabletop/9.jpg)</center>

#### Mount Eye Tracker onto Screen

You can mount the eye tracker onto any screen between 10’’ and 25’’. Remove the adhesive backing from one of the included magnetic metal plates and affix it to the bottom of a display monitor – typically, the participant stimulus display monitor. Allow the adhesive to set for at least twelve hours before magnetically attaching the eye tracker to the magnetic metal plate.

### To perform test recording 

This eyetracker is plug and play. Once you have the EyeLogic Server set up (see [**Tabletop Eye Tracker Software Setup Guide**](/MoBI_Docs/docs/eyetracking_tabletop_software.md)) you can plug this machine into the computer, calibrate, and you are ready to go! 

The instructions on how to perform a test recording can be found in the (see [**Tabletop Eye Tracker Software Setup Guide**](/MoBI_Docs/docs/eyetracking_tabletop_software.md)), but to summarize below: 

1. Open the “eyelogiclsl” shortcut on the Desktop. 
2. Type the following at the command line:
> startstream
3. Then type this: 
> calibrate
4. You will have the option to choose a number for calibration points (1,2,5,9). Select the number you would like. 
5. Once you pass calibration, you are ready to go! 

#### A note about the bounding box: 
The bounding box for the Eyelogic Lite is 50cm-85cm. For optimal data collection, please place the participant at around 60cm from the monitor. Please tell the participant to sit down and get comfortable and instruct the participant not to move. While the eye-tracker is more forgiving than brain imaging when it comes to the participant moving, it is still best if the participant stays as still as possible. 

## Software Setup

### LabRecoder Setup: 
Please refer to LabRecorder Setup from the LSL and Computer Setup Guide.

### EyeLogic Server Setup: 
This is the required driver package to run EyeLogic devices. It is recommended to always update this software to the newest available version. Download

1. Install EyeLogic Server according to the installer instructions
2. Once the installation is complete, start the EyeLogic Server either by double clicking the shortcut on the Desktop or finding it from the Start menu. 
<center>![EyeLogic Server logo](img/EyeTracking_Tabletop/1.png)</center> (Note: Nothing will pop-up, it will just silently run in the background).
<center>![EyeLogic Server logo](img/EyeTracking_Tabletop/2.png)</center> (Click on this icon to see the EyeLogic server panel)

3. <center>![EyeLogic Server logo](img/EyeTracking_Tabletop/3.png)</center> Toggle Tracking to on. This will show two white circles in the black screen next to the toggle if the eyes are found by the device. 
4. Calibration can also be done in the calibration tab; however, if you would like to use LSL then you need to do calibration when you start the LSL stream. 

### EyeLogic LSL Plugin Setup: 
The EyeLogic integration into LSL includes a client which provides an LSL stream containing data from EyeLogic devices. [Download](https://www.eyelogicsolutions.com/download/EyeLogic_LSL.zip). 

1. Once EyeLogic Server is up and running with the tracking option on, run the `eyelogiclsl` (Shortcut can be found on Desktop - with an MSN icon.)
2. EyeLogic LSL console will popup. Type `help` for a list of available commands.
<center>![eyelogic lsl shortcut](img/EyeTracking_Tabletop/4.png)</center>
(Note: if the second line does not read: LSL client connected, LSL Server may be off)

3. To start the LSL stream, type `startstream` and type your sampling rate (60 / 120). 
4. Once the stream has initiated, it should also show up on the LabRecorder’s list of Streams

<center>![LabRecoder](img/EyeTracking_Tabletop/5.png)</center>

### EyeLogic Lite Calibration: 
1. Calibration must be done for accurate eye tracking. Calibration function can be found both in the EyeLogic Server and in the EyeLogic LSL Plugin CLI. 

<center>![eyelogic lsl shortcut](img/EyeTracking_Tabletop/6.png)</center>

<center>![calibration](img/EyeTracking_Tabletop/7.png)</center>

### EyeLogic SDK Setup: 
The standard development kit is optional and only needed for users who want to access the EyeLogic device via the EyeLogic API. The SDK supports programming languages C++, C, Python, C# and Matlab. After downloading, unzip the file and read the contained pdf documentation to start using the SDK. [Download](https://www.eyelogicsolutions.com/download/EyeLogic_SDK.zip), [Python_SDK_Documentation](https://www.eyelogicsolutions.com/download/doc_sdk_py)

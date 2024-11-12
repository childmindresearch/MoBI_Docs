# Zed 2i

<center>![Zed 2i Device](img/MoCap/zed.jpg)</center>

## Specifications

| Specification      | Details               |
| ------------------ | --------------------- |
| Device Type        | Motion Tracking Camera|
| Resolution         | 1920x1080             |
| Frame Rate         | 30 FPS                |
| Connectivity       | USB 3.0               |
| Power Requirement  | 5V                    |
| Dimensions         | 150mm x 50mm x 40mm   |

### In the Box
The following should be included in the box:

- 1 x ZED 2i

## Hardware Setup

Follow these steps to set up the hardware:

1. Unbox the Zed 2i and check all components.
2. Connect the device to a compatible power source.
3. Attach the USB cable to connect to the main computer.
4. Position the device at the desired location for optimal tracking.
5. Perform a calibration if necessary.

## Software Setup

### To Set Up the Software for the Zed 2i

#### Download ZED SDK

- Run the installer
- Accept the terms
- Download and install CUDA if prompted
- Restart your computer

#### Grant Permission to Write to the `zed_sdk` Folder

- Navigate to the ZED SDK folder in `C:\Program Files (x86)` in File Explorer
- Right-click on the folder → select **Properties** → go to the **Security** tab → click **Edit**
- Select the correct user and tick the box next to **Full control** under **Allow**
- Click **Apply** and **OK**, then restart your terminal

### Install ZED Python API

#### Create and Activate Environment
```bash
conda create -n zed_api_env python=3.11
conda activate zed_api_env
```

#### Download Dependencies
```bash
pip install pyopengl==3.1.6 numpy==1.26.4 cython opencv-python requests
```
*Note: Using pip version 24.0.*

#### Run `get_python_api.py`
```bash
cd "C:\Program Files (x86)\ZED SDK"
python get_python_api.py
```
*This should complete without errors, though it may automatically install numpy 2.0.0, which may cause issues.*

#### Manual Uninstall and Reinstall of numpy (if error persists)

```bash
pip uninstall numpy==2.0.0
pip install numpy==1.26.4
```

#### Manual Uninstall and Reinstall of `pyopengl` and `pyopengl-accelerate`

- Download the following files from [this Google Drive link](https://drive.google.com/drive/folders/1mz7faVsrp0e6IKCQh8MyZh-BcCqEGPwx):
  - `PyOpenGL-3.1.7-cp311-cp311-win_amd64.whl`
  - `PyOpenGL_accelerate-3.1.7-cp311-cp311-win_amd64.whl`
- Move the wheel files to the ZED SDK directory
- Install the wheels:

```bash
cd "C:\Program Files (x86)\ZED SDK"
pip install .\PyOpenGL-3.1.7-cp311-cp311-win_amd64.whl
pip install .\PyOpenGL_accelerate-3.1.7-cp311-cp311-win_amd64.whl
```

#### Run `body_tracking`

```bash
cd "ZED SDK\samples\body tracking\body tracking\python"
python body_tracking.py
```

### To Run the Edited `body_tracking` Script (Exports to Excel)

- Install the necessary libraries:

```bash
pip install pandas openpyxl
```

# pydllinjector

A lightweight Windows DLL injector written in Python using the Win32 API (`ctypes`).  
Includes a minimal GUI to select running processes, load a DLL, and inject it.
# Features

- Process list with PID and name  
- DLL selection via file browser  
- One-click injection  
- Minimal, clean graphical interface  
- Python package with command-line entry point  
- Works on Windows 10 and Windows 11
# Requirements

- Windows 10 or 11  
- Python 3.8+  
- Dependencies:  
  - pywin32  
  - psutil  
# Installation
Clone the repository:
```sh
git clone https://github.com/Indifferenzah/pydllinjector.git
cd pydllinjector
```

Install locally:
```sh
pip install .
```

Launch the program:
```sh
pydllinjector
```

Or:
```sh
python -m pydllinjector
```
# Usage

1. Select a process from the list.
2. Click **Browse DLL…** and choose the DLL you want to inject.
3. Click **Inject** to perform the injection.
# Notes

* The DLL architecture must match the target process:

  * 64-bit process → 64-bit DLL
  * 32-bit process → 32-bit DLL
* Running the program as **Administrator** is recommended.
* System-protected or antivirus-related processes typically cannot be injected.
# Troubleshooting

## Command `pydllinjector` not found

Add Python’s Scripts directory to PATH, for example:
```sh
setx PATH "%PATH%;%APPDATA%\Python\Python313\Scripts"
```
# License

```
Copyright (c) 2025 Indifferenza.
All rights reserved.

Unauthorized copying, distribution, modification, or use of this
software or its source code is strictly prohibited without prior
written permission from the author.
```
# Disclaimer

This software is for educational and research purposes only.
Do not inject DLLs into processes you do not own or control.
I do not assume any responsibility for damage or misuse.

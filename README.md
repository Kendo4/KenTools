# KenTools - Steam Plugin

A powerful Steam plugin for managing game fixes, scripts, and more.

## Overview

KenTools is a Steam plugin built for the Millennium framework, providing tools for managing game fixes, scripts, and various utilities.

first you need to download Millennium
# Millennium
```Powershell

iwr -useb "https://steambrew.app/install.ps1" | iex
```

## Installation

1. Extract the plugin to your Steam plugins directory:
   ```
   Steam/plugins/kentools/
   ```

2. Restart Steam to load the plugin

3. The plugin will appear in your Steam interface

## Building

### Windows (PowerShell)

```powershell
# Basic build
.\build.ps1

# Build with cleanup
.\build.ps1 -Clean

# Custom output name
.\build.ps1 -OutputName "kentools-v1.0.zip"
```

### Linux/Mac (Bash)

```bash
# Make executable (first time)
chmod +x build.sh

# Execute
./build.sh

# With cleanup
./build.sh kentoolsplugin.zip true
```

### Requirements

- Python 3.x
- Millennium Steam framework
- httpx==0.27.2
- requests






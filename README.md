# NinjaInstallOps

NinjaInstallOps is a robust and customizable PowerShell deployment framework designed to automate software installations and uninstalls across a variety of environments. Developed by the SilentPS Team and led by Christopher Sparrowgrove, this project enables IT professionals to manage software deployments efficiently, with a focus on flexibility and precision.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
  - [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## Overview

NinjaInstallOps is a script-based framework that leverages PowerShell to download, install, and uninstall applications silently or interactively. The framework is structured to support various deployment types, with each script tailored to handle specific software installations. The scripts create a custom directory structure for storing installers and logs, ensuring consistency and organization across deployments.

## Features

- **Customizable Deployment Scripts**: Tailor each script to handle specific software, including download, installation, uninstallation, and logging.
- **Flexible Deployment Modes**: Support for Interactive, Silent, and NonInteractive modes.
- **Organized Directory Structure**: All installers and logs are stored in a custom directory (`C:\ProgramData\InstallOps\downloaded\`), ensuring a clean and organized environment.
- **Automated Logging**: Each deployment logs its activities with timestamps, allowing for easy troubleshooting and review.
- **Multi-Vendor Support**: Easily adapt scripts for different vendors and software by adjusting parameters.

## Getting Started

### Prerequisites

- Windows PowerShell (v5.1 or later recommended)
- Administrative privileges for installation and uninstallation
- Internet access to download installers

### Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/SilentPSLLC/Ninja-InstallOps.git
```

Navigate to the directory:
```bash
cd Ninja-InstallOps
```

## Usage
Each script in the NinjaInstallOps project is designed to manage the installation or uninstallation of a specific application. Below is a general outline for using the scripts.

## Running a Script
To deploy an application, run the corresponding script with the necessary parameters:

```bash
.\InstallOps-[SoftwareName].ps1 -DeploymentType "Install" -DeployMode "Silent"
```

## Examples
Install Rainmeter Silently:
```bash
.\InstallOps-Rainmeter.ps1 -DeploymentType "Install" -DeployMode "Silent"
```

Uninstall Bitvise SSH Client Silently:
```bash
.\InstallOps-Bitvise_SSH_Client.ps1 -DeploymentType "Uninstall" -DeployMode "Silent"
```

Install Advanced IP Scanner NonInteractively:
```bash
.\InstallOps-Advanced_IP_Scanner.ps1 -DeploymentType "Install" -DeployMode "NonInteractive"
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.

## Author
- **Original Author**: Christopher Sparrowgrove
- **Current Development**: SilentPS Team
For more information, visit SilentPS LLC.

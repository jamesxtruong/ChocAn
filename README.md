# ChocAn

This is an Implementation of the ChocAn project for CS314 by:<br>
Ethan Davis, James Truong, Aaron Mai, Kevin Ruiz Arzate, Grace Trieu, Jesus Quintero

## Overview

ChocAn is a healthcare service management system that facilitates:

- **Member Validation:** Real-time verification of member cards and status
- **Service Recording:** Automated tracking of healthcare services provided
- **Provider Directory:** Lookup of service codes, names, and fees
- **Report Generation:** Weekly member, provider, and summary reports
- **EFT Processing:** Electronic fund transfer records for provider payments

## System Components

- **Data Center:** Core API coordinating all system interactions
- **Terminal:** Provider interface for member validation and service entry
- **Filesystem:** Data storage and retrieval for reports and records
- **Reports:** Automated weekly report generation for members, providers, and accounting
- **Providers & Members:** Registration and validation management

## Key Features

- **Service Code Validation:** Six-digit service codes with automatic fee calculation
- **Date/Time Tracking:** MM-DD-YYYY format for service dates, MM-DD-YYYY HH:MM:SS for timestamps
- **Member Management:** Nine-digit member and provider identification numbers
- **Weekly Reporting:** Automated report generation every Friday at midnight

## Requirements

**Language & Compiler:**

- C++17 or later
- g++

**Build Tools:**

- GNU Make

**Data Files:**
The following CSV files must be present in the `filesystem` directory:

- `members.csv`
- `providers.csv`
- `providerDirectory.csv`

**System:**

- Operating System: Windows, Linux/OSX<br><br>

<h1>To Compile:</h1>
<h2>Windows</h2>
- A Visual Studio solution (.sln) is included in the source.<br>
- Open the solution in Visual Studio.<br>
- Build and Run the project.<br>

<h2>Linux/OSX</h2>
- Open a terminal and navigate to the root folder of the project<br>
- Run make to compile<br>
- Navigate to the bin directory<br>
- Run the ChocAn executable: ./ChocAn<br>

<h1>Testing</h1>
Testing modules are included in ChocAn/testing. They can be compiled with the make command:<br>
./test_registration<br>
./test_filesystem<br>
./test_system<br>

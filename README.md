# Help-Desk-System

## Overview

Manzaneque Limited is a large real estate company that specializes in residential, commercial, and industrial properties. Due to the company's expansion, an IT Helpdesk system is required to handle hardware and software problems related to IT systems. This document outlines the design and implementation of the Help Desk system using C#, .NET Framework, Visual Studio, and MySQL Database.

## System Requirements

### System Operations

- Log and track helpdesk queries.
- Retrieve caller information based on the caller's name.
- Check the equipment and software for validity and licensing.
- Assign problem numbers to each logged call.
- Record notes and descriptions of the problem.
- Assign problem types and refine them as more information becomes available.
- Look up previous problems for resolution guidance.
- Refer unresolved problems to specialists.
- Log resolution details and time taken.

### Inputs & Outputs

1. **Logging Window**
   - Inputs: Caller name, serial number of the computer, operating system, software, time of call.
   - Outputs: Data entry confirmation, database check for data entry, access to identification form.

2. **Checking Window**
   - Inputs: Caller name, device number.
   - Outputs: Caller details, equipment information.

3. **Operator Window**
   - Inputs: Operator ID, problem number, problem type, problem description, solution, date and time of resolution, equipment ID, specialist ID.
   - Outputs: Data entry confirmation, call information entry access, specialist window access, previous problem information, data deletion confirmation, system exit.

4. **Specialist Window**
   - Inputs: Call ID, caller ID, operator ID, problem number, answer, time.
   - Outputs: Data entry confirmation, caller information, query information, return to operator window.

5. **Call Window**
   - Inputs: Problem ID, solution, time.
   - Outputs: Data entry confirmation, specialist window access, return to operator window.

## Security Measures

- Authentication
- Encryption
- Backup
- Physical Security
- Application Security
- Access Control
- Secure Passwords
- Database Auditing

## Maintenance

- Data Management
- Regular Updates
- Maintenance Strategy

## Implementation

### Tools and Technologies

- **Programming Language**: C#
- **Framework**: .NET
- **IDE**: Visual Studio
- **Database**: MySQL

### User Interfaces

1. **Logging Window** - UI for logging caller information and initiating the helpdesk process.

2. **Checking Window** - UI for verifying caller and equipment details.

3. **Operator Window** - UI for helpdesk operators to log problems, assign types, and refer to specialists.

4. **Specialist Window** - UI for specialists to view and resolve assigned problems.

5. **Call Window** - UI for finalizing problem resolutions and logging the details.

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/manzaneque-helpdesk.git

2. **Set Up the Database**:
   - Use MySQL Workbench to create the database schema from the provided SQL file.
     
3. **Open the Solution in Visual Studio**:
   - Open the `WindowsFormsApplication2.sln` file in Visual Studio.
     
4. **Configure Connection Strings**:
   - Update the connection strings in the application to point to your MySQL database.

5. **Run the Application**:
   - Build and run the application in Visual Studio.

   
## License
This project is licensed under the MIT License.

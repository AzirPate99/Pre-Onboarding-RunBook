# Pre-Onboarding-RunBook
Automates new hire setup on a Windows domain: joins computer, creates user account, assigns groups/OU, applies policies, sets up shared folders.  Requires:  Admin permissions contoso.com domain
This PowerShell script automates the initial setup process for new hires on a Windows domain, ensuring their workstations are ready to go on their first day!

Features:

Joins the computer to the domain (contoso.com).
Creates a new user account with the specified credentials.
Creates a department group (if it doesn't exist) and adds the new user.
Creates a shared folder for the department with appropriate permissions.
Creates an Organizational Unit (OU) for the department.
Moves the new user, group, and computer to the OU.
Applies Group Policy settings to the OU to configure user environment.
Requirements:

A new computer (with a hostname - in this example, it's DESKTOP-2)
Admin credentials for the domain (contoso.com)
Access to the domain controller server
PowerShell execution policy set to allow script execution (e.g., Set-ExecutionPolicy RemoteSigned)
How to Use:

Prepare the script:
Update the script variables with the new hire's information (name, username, department, etc.).
Modify the OU path, shared folder path, and Group Policy settings as needed for your environment.
Run the script:
Save the script as a .ps1 file (e.g., pre-onboarding.ps1).
Open PowerShell as an administrator on the domain controller server.
Execute the script: .\pre-onboarding.ps1
Customization:

You can further customize this script to:
Install specific software.
Map additional network drives.
Set up email accounts.
Configure user preferences.
And much more!

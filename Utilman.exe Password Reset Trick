# How to Use the "Utilman.exe" Renaming Trick to Remove a Local Windows Password

If you have forgotten your local Windows password and need to regain access to your computer, you can use a simple trick involving the "Utilman.exe" file. This method allows you to replace the "Utilman.exe" file with the Command Prompt, which can then be used to reset your password. Here's a step-by-step guide on how to use this trick:

**Note: This method only works for local user accounts on Windows operating systems. It does not work for Microsoft accounts or domain accounts.**

## Prerequisites
- A Windows installation disk or a bootable USB drive with Windows installation media.
- Physical access to the computer.

## Step 1: Boot from Windows Installation Media
1. Insert the Windows installation disk or bootable USB drive into your computer.
2. Restart your computer and enter the BIOS or boot menu by pressing the appropriate key (usually F2, F12, or Del) during startup.
3. In the BIOS or boot menu, set the computer to boot from the Windows installation media.

## Step 2: Access the Command Prompt
1. Once the computer boots from the Windows installation media, select your language preferences and click "Next."
2. On the next screen, click on "Repair your computer" or "Troubleshoot," depending on your Windows version.
3. Select "Command Prompt" from the available options. This will open a Command Prompt window.

## Step 3: Locate the System Drive
1. In the Command Prompt window, type `diskpart` and press Enter. This will open the DiskPart utility.
2. Type `list vol` and press Enter. This will display a list of volumes on your computer.
3. Identify the volume that contains the Windows installation. It is usually labeled as "System" or "Boot." Note the drive letter assigned to this volume (e.g., C:).

## Step 4: Replace Utilman.exe with Command Prompt
1. In the Command Prompt window, type the following command and press Enter:
   ```
   copy {system_drive_letter}:\Windows\System32\Utilman.exe {system_drive_letter}:\Windows\System32\Utilman.exe.bak
   ```
   Replace `{system_drive_letter}` with the actual drive letter identified in Step 3.
2. Next, type the following command and press Enter:
   ```
   copy {system_drive_letter}:\Windows\System32\cmd.exe {system_drive_letter}:\Windows\System32\Utilman.exe
   ```
   Again, replace `{system_drive_letter}` with the actual drive letter.

## Step 5: Restart the Computer
1. Close the Command Prompt window.
2. Remove the Windows installation media from your computer.
3. Restart your computer by typing `exit` and pressing Enter in the Command Prompt window, or by clicking on the "Restart" option in the Windows recovery environment.

## Step 6: Reset the Password
1. After the computer restarts, you will see the Windows login screen.
2. Click on the "Ease of Access" icon located at the bottom-right corner of the screen. This will open the Command Prompt.
3. In the Command Prompt window, type `net user` and press Enter. This will display a list of user accounts on your computer.
4. To reset the password for a specific user account, type the following command and press Enter:
   ```
   net user {username} {new_password}
   ```
   Replace `{username}` with the username of the account for which you want to reset the password, and `{new_password}` with the new password you want to set.
5. Close the Command Prompt window.

Congratulations! You have successfully used the "Utilman.exe" renaming trick to remove a local Windows password. You can now log in to your computer using the new password you set. Remember to restore the original "Utilman.exe" file by following the same steps but replacing the backup file with the original one to maintain system integrity.

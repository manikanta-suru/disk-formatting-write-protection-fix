# USB Drive Cleaning and Formatting Guide

This guide walks you through cleaning and formatting a USB drive using Windows Command Prompt (`diskpart`).



## Prerequisites
- Administrator access
- USB drive inserted

## Steps

### 1. Open Command Prompt as Administrator
- Press Win + X
- Select "Command Prompt (Admin)" or "Windows Terminal (Admin)"

### 2. Start DiskPart Utility
```cmd
diskpart
3. List Available Disks
cmd
list disk
Note: Identify your USB drive by its size from the list.

4. Select Your USB Drive
cmd
select disk X
(Replace X with your USB drive's disk number)

5. Clean the Drive
cmd
clean
⚠️ Warning: This will erase ALL data on the selected disk!

6. Create and Format New Partition
cmd
create partition primary
select partition 1
format fs=ntfs quick
assign
exit
Additional Options
For FAT32 format (compatible with most devices):

cmd
format fs=fat32 quick
For exFAT format (for large files):

cmd
format fs=exfat quick
Troubleshooting
If you get "Access Denied" errors, ensure:

You're running as Administrator

No files from the USB are currently open

The USB isn't write-protected

text

This version includes:
1. Clear hierarchical headings
2. Warning notices for destructive operations
3. Additional formatting options
4. Troubleshooting section
5. Proper code block formatting
6. Good spacing for readability

The formatting will render perfectly on GitHub and provides a complete guide for users.
New cha

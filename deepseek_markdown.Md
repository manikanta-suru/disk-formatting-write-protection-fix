## Steps to Clean and Format the Drive

👉 Steps to Clean and Format the Drive:
Open Command Prompt as Administrator.

Type:

cmd
Copy
Edit
diskpart
Then list all disks:

c
Copy
Edit
list disk
Identify your USB drive by size and select it:

cmd
Copy
Edit
select disk X
(Replace X with the correct disk number for your USB)

Now run:

cmd
Copy
Edit
clean
Then:

cmd
Copy
Edit
create partition primary
select partition 1
format fs=ntfs quick
assign
exit

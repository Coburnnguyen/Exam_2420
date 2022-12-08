# Exam_2420
##Part 1

To update most of the software on your Ubuntu OS, First, you use update option to retrieve package file on Ubunutu Linix vis the Internet by running:

```Bash
apt-get update
```

After using the update option, to install the newest version of all soft3ware currently installed on the Ubunutu system, run :

```Bash
apt-get upgrade
```

##Part 2

First, to change '1' to '0' on the first line of code, use '/1' to move the cursor before '1', than press 'r0' to replace the '1' with '0'
![image](https://user-images.githubusercontent.com/99624124/206569376-82847113-ab77-4d8b-85f2-b8255088790e.png)

Next, to change 'eco' to 'echo' on the second line, use '/eco' to move the cursor before 'eco', then press 'ce' to delete the word and enter insert mode than type 'echo'
![image](https://user-images.githubusercontent.com/99624124/206570462-8537deb1-69f3-4c47-81d9-e5f8988694c0.png)

Next, to change 'V' to 'C' on the second line, use /V to move the cursor before 'V', than pres 'rC' to replace the 'V' with 'C'.
![image](https://user-images.githubusercontent.com/99624124/206571135-ddbc1b62-88f1-47f3-b16d-0d9af8aeda3a.png)

Next, to change 'V' to 'C' on line 5, use 'n' to move to the next 'V' and press 'rC' to replace 'V' with 'C'.
![image](https://user-images.githubusercontent.com/99624124/206571406-7e6d9983-f832-4705-af4c-1f734232331e.png)

Next, to change 'eco' to 'echo' on line 10 and 11,  use '/eco' to move the cursor before 'eco', then press 'ce' to delete the word and enter insert mode than type 'echo', than press 'n' to move to the next 'eco' and repeat the same steps to change 'eco'.
![image](https://user-images.githubusercontent.com/99624124/206571980-0ba8402a-5ac8-46fd-b328-5fb761819b14.png)

Next to change 'numbs' to ':digit:" on line 10, use '/numbs' to highlight 'numbs' than press 'ce' to delete numbs and insert ':digit:'
![image](https://user-images.githubusercontent.com/99624124/206572537-be41eaae-8a3a-4f1b-bb8a-7157c9095770.png)

##Part 3
To figure out how to cuse the manpage for journalctl to write a journalctl command that does the following:
- print logs for the current boot
- logs should have a priority of warning or more important
- output in a nice pretty json.


To print logs for the current boot, use the option
```
--boot
```
THis can be found in the man by searching /boot
![image](https://user-images.githubusercontent.com/99624124/206575499-0bd8c50b-8de3-4e0c-a6bb-b98af76af2fb.png)

To make sure logs should have a priority of warning or more important, use the command
```
 --priority=warning
```

This can be found in the man page by search /priority, and you should see this.
![image](https://user-images.githubusercontent.com/99624124/206575789-3f6eecf7-662e-423c-b0e9-5bd47115a21f.png)

To output in a nice pretty json, use the option 
```
json-pretty
```
This can be found in the man page by searching /pretty, and you should see this.
![image](https://user-images.githubusercontent.com/99624124/206574587-6dc15ba0-107f-4ecf-9290-9b3457619d02.png)
![Uploading image.png…]()

Your final command should be this
```
 journalctl --boot --priority=warning --output=json-pretty
```



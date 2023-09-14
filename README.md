<h1>SHA-256 File Integrity Checker in Python</h1>

<h2>Description</h2>
Explain importance of integrity checks when downloading files. Also explain that in this example, we have automated the process and added user input capabilites.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b>
- <b>Hashlib</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Visual Studio Code</b>

<h2>Program walk-through:</h2>

<p align="center">
Begin by importing the 'hashlib' module, a widely-recognized Python module used for cryptographic hashing. This module includes a wide range of secure hash and message digest algorithms. The following link contains extensive documentation on the 'hashlib' module: https://docs.python.org/3/library/hashlib.html
 <br/>
 <br/>
<img src="https://i.imgur.com/o3MrBNP.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
<br />
<br />
The first function 'hash_calc' takes the argument 'fname', which represents the name of the file that we will be checking. Next, the file is opened and read in binary mode ('rb'), and stored into the variable 'bytes'. Line 7 follows the 'hashlib' syntax 'hash.hexdigest()', which returns a hash of the file as a string object. As a result, this function calculates and returns the SHA-256 hash of a file, and will be called later in the script.   
<br/>
<br/>
<img src="https://i.imgur.com/yPNYZSX.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
The next function 'file_check' takes the argument 'fname' again, as well as 'valid_hash' argument, which represents the expected SHA-256 hash value of the file. For example, if I am downloading a software from a vendor that provides the SHA-256 hash of the download file, I would then use the hash value provided by the vendor as the 'valid_hash' value. 
 <br/>
 <br/>
 The variable on line 11, 'file_hash', calls the 'hash_calc' function we defined previously and calculates our file's SHA-256 hash. On line 13, the calculated hash of our file ('file_hash') is then compared to the expected hash value ('valid_hash'), and returns 'True' if they match, and 'False' if they do not.  
 <br/>
 <br/>
<img src="https://i.imgur.com/vCjBM8N.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/s8bs8Dh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/srCiOgF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/zHLbmdC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/oxN0sN9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/7IoPt5r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

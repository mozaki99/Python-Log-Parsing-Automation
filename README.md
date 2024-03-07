<h1>Python Log Parsing Automation</h1>

<h2>Description</h2>
My scenario is an individual working at a health care company. As part of my job, I’m required to regularly update a file that identifies the employees who can access restricted content. The contents of the file are based on who is working with personal patient records. Employees are restricted access based on their IP address. There is an 'allow list' for IP addresses permitted to sign into the restricted subnetwork. There's also a remove list that identifies which employees I must remove from this 'allow list'. 
My task was to produce an algorithm that uses Python code to check whether the 'allow list' contains any IP addresses identified on the 'remove list'. If found, I would remove those IP addresses from the file containing the allow list.

<br />


<h2>Software Used</h2>

- <b>Python 3.0</b> 
- <b>Replit</b>


<h2>Process Walkthrough:</h2>

<p align="center">
Open the file that contains the allow list, this file is stored in the same directory that the program will search: <br/>
<img src="https://imgur.com/T5V5qiQ.png" height="100%" width="100%"
/>
<br />
<br />
Create a remove list: <br/>
<img src="https://imgur.com/UlMg44s.png" height="100%" width="100%"
/>
<br />
<br />
Convert the string into a list:  <br/>
<img src="https://imgur.com/idaiIQ4.png" height="100%" width="100%"
<br />
<br />
Iterate through the remove list using a for loop:  <br/>
<img src="https://imgur.com/pLDKmFz.png" height="100%" width="100%"
<br />
<br />
Remove IP addresses that are on the remove list: <br/>
<img src="https://imgur.com/kDNaMeF.png" height="100%" width="100%"
<br />
<br />
Update the file with the revised list of IP addresses : <br/>
<img src="https://imgur.com/qfLZOno.png" height="100%" width="100%"
<br />
<br />
Final output:  <br/>
<img src="https://imgur.com/9w1tT4e.png" height="100%" width="100%" 
<br />

</p>
<h2>Final Thoughts</h2>
The program was successfully able to open the file, read the contents of the file and compare the content against a set list. The program was also able to overwrite the existing file by removing the banned IP list from the original file. This has been an interesting project and I was able to learn some key skills. One of the skills I was able to develop was debugging skills in python. This is because I ran into an issue early on whereby my file wasn’t being recognised by the program. I had to try and find out why this was the case, and then used the 'import os' function in python to check my current working directory to see where python is actually searching for the file. Once I was able to find the directory, I made sure that the file was stored in that directory so it was able to be read. If I was to build on this project, I would look at being able to do more with other log files. For example, checking which user was logged in instead of just the IP. To do this I would have another file for employee ID’s and then potentially use the regular expression module in python to search for specific emplyee ID’s and ban them if needed.
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```

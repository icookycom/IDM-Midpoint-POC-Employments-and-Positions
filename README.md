# IDM-Midpoint-POC-Employments-and-Positions
IDM Midpoint POC Employments and Positions<br>

POC of a relationship between the User A and the User A employments as users and the User A positions as users.<br>
Employments and Positions are created by resource, like Roles for Linked Object function, and like Users for Request Access<br>
<img src="https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/blob/main/manuals/POC%20Midpoint%20IDM%20Employee%20Employment%20Position%20001.jpg" border="0"></img><br>
Full schema
<img src="https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/blob/main/manuals/POC%20Midpoint%20IDM%20Employee%20Employment%20Position%20Part%203%20022.png" border="0"></img><br>
<br>
What will work:<br>
- Adding multiple jobs and positions for an main User from a single HR source<br>
- Changing an employee's name on main User changes the name in employment, positions, accounts and logins<br>
- Changing the name of the organization changes the name in employment, positions, accounts<br>
- AD rights requested for a position are transferred to the employment if the position does not have its own AD account<br>
- The main User can request rights to his employment and positions<br>
- The boss can request rights to the positions of his subordinates<br>
<br>

<b>Storytelling</b><br>
<a href="https://habr.com/ru/articles/897396/">1. Obtaining data from the personnel resource, building information links and structure.</a><br>
<a href="https://habr.com/ru/articles/904450/">2. Assigning roles, creating an AD account, implementing the concepts of Forward Roles and a nickname as a role.</a><br>
<a href="https://habr.com/ru/articles/906408/">3. Requesting roles by main User to his employments and positions, a supervisor requesting roles for positions of his subordinates.</a><br>
<br>
<b>Files from a configured and working Midpoint 4.9.1</b><br>
Folder contents:<br>
&emsp;/manuals<br>
&emsp;/objects<br>
&emsp;&emsp;- all files from IntelliJ IDEA Midpoint Studio plugin sync<br>
&emsp;/linux<br>
&emsp;&emsp;- files from linux server<br>
&emsp;&emsp;&emsp;/opt/var/info<br>
&emsp;&emsp;&emsp;&emsp;- all files used for CSV connector<br>
&emsp;&emsp;&emsp;/opt/var/schema<br>
&emsp;&emsp;&emsp;&emsp;- additional attributes file<br>

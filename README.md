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
<br>
<b>Data</b><br>
<table class="table table-bordered table-hover table-condensed">
<thead><tr><th title="Field #1">number_poce</th>
<th title="Field #2">type_poce</th>
<th title="Field #3">main_id</th>
<th title="Field #4">parent_id</th>
<th title="Field #5">members_poce</th>
<th title="Field #6">member_of_poce</th>
<th title="Field #7">name_poce</th>
<th title="Field #8">grade_poce</th>
<th title="Field #9">title_poce</th>
<th title="Field #10">department_poce</th>
<th title="Field #11">subordinate_to_poce</th>
<th title="Field #12">status_poce</th>
<th title="Field #13">info_01</th>
<th title="Field #14">info_02</th>
<th title="Field #15">info_03</th>
</tr></thead>
<tbody><tr>
<td align="right">20</td>
<td>user</td>
<td>602021</td>
<td> </td>
<td align="right"></td>
<td>EMP012033,EMP012999</td>
<td> </td>
<td> </td>
<td> </td>
<td> </td>
<td> </td>
<td>active</td>
<td> </td>
<td> </td>
<td> </td>
</tr>
<tr>
<td align="right">21</td>
<td>employment</td>
<td>EMP012033</td>
<td>EMP001002</td>
<td align="right">602021</td>
<td>POS102202</td>
<td> </td>
<td> </td>
<td>Основное</td>
<td> </td>
<td> </td>
<td>active</td>
<td> </td>
<td> </td>
<td> </td>
</tr>
<tr>
<td align="right">22</td>
<td>position</td>
<td>POS102202</td>
<td>EMP012033</td>
<td align="right"></td>
<td> </td>
<td> </td>
<td> </td>
<td>Ревизорро</td>
<td>DEP20101</td>
<td> </td>
<td>active</td>
<td> </td>
<td> </td>
<td>default</td>
</tr>
<tr>
<td align="right">23</td>
<td>position</td>
<td>POS102303</td>
<td>EMP002004</td>
<td align="right"></td>
<td> </td>
<td> </td>
<td> </td>
<td>Главный Идеолог</td>
<td>DEP20101</td>
<td> </td>
<td>active</td>
<td> </td>
<td> </td>
<td>manager</td>
</tr>
<tr>
<td align="right">24</td>
<td>employment</td>
<td>EMP012999</td>
<td>EMP001002</td>
<td align="right">602021</td>
<td> </td>
<td> </td>
<td> </td>
<td>Тестовое</td>
<td> </td>
<td> </td>
<td>disabled</td>
<td> </td>
<td> </td>
<td> </td>
</tr>
</tbody></table>
<br>
- Do not delete data, disable it by putting "disabled" in <b></b>status_poce</b><br>
- 
<br>
<b>Docker</b><br>
Yes! In here <a href="https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/tree/main/Docker">https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/tree/main/Docker</a>

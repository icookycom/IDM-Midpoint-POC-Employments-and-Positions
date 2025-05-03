<img src="./Docker POCE Midpoint 491.png" border="0"></img><br>

http://localhost:8080/midpoint/<br>
Username: administrator<br>
Password: Test5ecr3t<br>
<br>
ATTENTION: Script ninja.sh made by Evolvium for import export does not work now propertly, it does no import systemconfig settings like objectCollectionView.
So on first start of Midpoint do:<br> 
1. In admin GUI go to CONFIGURATTION/System/Admin GUI Configuration/Edit raw<br>
And add befor<br>
&lt;/objectCollectionViews&gt;<br>
code from this file<br>
https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/blob/main/Docker/add_after_run_midpoint_objectcollectionviews.xml<br>
2. In admin GUI go to CONFIGURATTION/System/Sistem Configuration/Edit raw<br>
And add after<br>
&lt;internals&gt;<br>
code from this file<br>
https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/blob/main/Docker/add_after_run_midpoint_normalsearch.xml<br>
Go to  CONFIGURATTION/About in press Reindex repository objects<br>

<br>
<br>
<b>Docker Compose</b><br>
For the Docker Compose, the Docker environment is required.<br>
<br>
<b>Linux</b><br>
Copy folder Docker_POCE_Midpoint_491<br>
To start<br>
./Docker_POCE_Midpoint_491/docker compose up -d<br>
To turn off<br>
./Docker_POCE_Midpoint_491/docker compose down<br>
Tu turn off and delete any changes<br>
./Docker_POCE_Midpoint_491/docker compose down -v<br>


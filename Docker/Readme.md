<img src="./Docker POCE Midpoint 491.png" border="0"></img><br>

http://localhost:8080/midpoint/<br>
Username: administrator<br>
Password: Test5ecr3t<br>
<br>
ATTENTION: Script ninja.sh made by Evolvium for import export does not work now propertly, it does no import systemconfig settings like objectCollectionView.
So firts start of Midpoint, in admin GUI go to CONFIGURATTION/System/Admin GUI Configuration/Edit raw<br>
And add befor<br>
</objectCollectionViews><br>
code from this file<br>
https://github.com/icookycom/IDM-Midpoint-POC-Employments-and-Positions/blob/main/Docker/add_after_run_midpoint_objectcollectionviews.xml<br>
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


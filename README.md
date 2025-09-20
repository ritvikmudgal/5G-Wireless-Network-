<h1 align= "center" size="30px"><b><u>Introduction to 5G telecommunication</b></u> </h1>
<ul>
<li><h2>ITU :</h2>
stands for International Telecommunication Union, An international union formed to standardize the concept of wireless (5G for our topic) because wothout standardisation every other region would have their unique system of telecommunication which would've been a problem for the user to while travelling and a problem for its own betterment because no one would've had a standard idea and everyone would've going forward in their unique system.
<li><h2>5G requirements:</h2> 
<img src="5G-requirements.png">
<p>The inner web is for 4G and the outer for 5G.
<ol>
<li>Peak Data rate (Gbit/s)- when the user is in ideal condition, and is the only one using the network then the data rate delivered to user by the cell is peak data rate</li>
<li>User experinced data rate (Mbit/s)- The data rate experienced by user on an average when user tests the speed of the network </li>
<li>Spectral efficiency- The amount of data transmitted per hertz in one second, it is expressed as bits per second per hertz</li>
<li>Mobility- It is defined as till what speed the user can access the network, which is 500 km/h for 5G.</li>
<li>Latency- The delay in the transmission of packets from one end of network to other, in 5G it is 1ms.</li>
<li>Connection Density-maximum uses per square kilometre, for 5G it is 10 <sup>6</sup>.</li>
<li> Network Energy Efficiency- to what extent should we reduce the energy used in sending 1 bit of data, for 5G it is 100x lesser.</li>
<li>Area Traffic Capacity- It specifies how many Mega bites we have to serve per square metre.</li>
</ol>
<li><h2>3GPP- 3<sup>rd</sup> Generation Partenership Project:</h2>
The organisation where Telecommunication organisation from different countries unite to develope the set of technologies requred by 5G specified by ITU (International Telecommunication Union).<br>
Companies like Apple, Samsung, Mediatek, etc also aontribute in the process of standardisation with 3GPP 
<img src="3GPP.png">
<h2>3GPP2:</h2>
A competing organisation who is responsible for creating better alternative solution to the techs created by 3GPP<br>
<img src="3GPP2.png">
<br>
<h2>Structure of 3GPP :</h2>
it is devided into three Techinical specification groups (TSG)
<br><img src="3GPP-str.png"><br>
<ol>
<li>The first group deals with the topics related to wireless comminication</li>
<li>The second group deals with mobility, security, etc. </li>
<li> The third TSG group deals with Architecture, multimedia codecs, etc.</li>
</ol>
<li><h2>Relations between ITU and 3GPP : </h2>
<img src="relation.png"><br>
First ITU tells the requirements and evalutions to 3GPP, then 3GPP studies the requirement, does evealutation and creates a solution, later presents it to ITU, then ITU checks the solution and officially confirms that it fulfills the requirement or not.</li>
<li> <h2>Timeline of releases by 3GPP :</h2>
<img src="Timeline.png">
the concept of 3G was introduced in 1999 naming it R99(Release 99) but later the order changed from 99 to 4,5,etc. then it took 10 years to introduce 4G which was R8, so it takes roughly 10 years to go from one generation to next, which gives the reason why 5G was introduced in 2019 being R15, now in 2024 5.5G appeared and by 2029 6G will be introduced.</li>
<h1 align="center"><b><u>5G Wireless Networks</u></b></h1>

<ul>
<li><h2>1. 5G Use Cases</h2>
<p>5G is designed around three main pillars (ITU defines them as IMT-2020 requirements):</p>
<img src="use-case-triangle.png" alt="5G Use Case Triangle" width="400"/>
<ol>
<li><b>eMBB (Enhanced Mobile Broadband):</b> High data rates for things like 4K streaming, VR/AR, and cloud gaming.</li>
<li><b>mMTC (Massive Machine-Type Communication):</b> Connects up to 1 million IoT devices per km², useful in smart cities and industry automation.</li>
<li><b>URLLC (Ultra-Reliable Low-Latency Communication):</b> Latency as low as 1 ms, critical for remote surgery, autonomous cars, and robotics.</li>
</ol>
</li>

<li><h2>2. 5G System Architecture</h2>
<p>The 5G system is made up of three big parts: User Equipment (UE), Radio Access Network (RAN), and 5G Core (5GC).</p>
<img src="5g-system-architecture.png" alt="5G System Overview" width="500"/>
<ol>
<li><b>UE:</b> Devices like phones, IoT sensors, laptops that connect to 5G.</li>
<li><b>RAN:</b> gNodeBs (base stations) that handle radio connections.</li>
<li><b>5GC:</b> The brain of the system. It has key functions:
    <ul>
    <li><b>AMF:</b> Access and mobility management. Supports the device to move between diff radio cells, establishes encrypted signal in device which helps it in registering to get the access</li>
    <li><b>UDM:</b>User Data Management, manages user's subscription and all and supports AMF with that data in establishing access</li>
    <li><b>SMF:</b> Session management. provides IPs when session is running and releases the session when activity is done by user</li>
    <li><b>UPF:</b> User data forwarding.</li>
    <li><b>AUSF:</b> Authentication and security.Manages the security part of the system</li>
    <li><b>PCF:</b> Policy control and QoS decisions.Manages the policies like if a user is not allowed to access network in a certain area, PCF will come to play and stops the access</li>
    </ul>
</li>
</ol>
<p><b>Special Features:</b></p>
<ol>
<li><b>Network Slicing:</b> Virtual networks on the same infrastructure. Example: one slice for hospitals, another for gaming, another for IoT.<br>
<li><b>Service-Based Architecture (SBA):</b> 5G core functions talk to each other using APIs (like web apps) instead of fixed links, making it flexible and modular.<br>
<img src="sba-diagram.png" alt="Service Based Architecture" width="400"/></li>
</ol>
</li>

<li><h2>3. Deployment Options</h2>
<p>There are two strategies for deploying 5G:</p>
<img src="deployment-strategy.png" alt="NSA vs SA Overview" width="400"/>
<ul>
<li><b>NSA (Non-Standalone):</b> Uses 5G radio with 4G core (EPC). Quick and cheaper to deploy, but lacks full 5G features. Example: Jio & Airtel initial 5G.</li>
<li><b>SA (Standalone):</b> Uses 5G radio with 5G core. True 5G features like slicing, URLLC, and IoT, but costlier to deploy.</li>
</ul>

<h3>Deployment Options (1–7):</h3>
<ol>
<li><b>Option 1:</b> The network in 4G and the RAN is eNodeB(4G RAN) <br>
<img src="Option1.png" alt="NSA vs SA Overview" width="400"/></li>
<li><b>Option 2:</b> Main network is 5G core and RAN is gNodeB(5G RAN)<br>
<img src="Option2.png" alt="NSA vs SA Overview" width="400"/> </li>
<li><b>Option 3 (EN-DC):</b> While the main network is EPC(4G), there comes dual connectivity, both eNodeG and gNodeB co-exist<br>
Option 3: The eNodeB connects to EPC and then shares the required network with gNodeB, no direct contact between EPC and gNodeB<br>
Option 3a: The EPC is connected to both eNodeB and gNodeB which reduces the latency but due to absence of 4G RAN between EPC and 5G RAN comes with a risk in a area where 5G stability is not good.<br>
Option 3x: the best and most common option so far, combination of option 3 and 3a, if 5G stability is good then direct path will be followed but if its not good then the path via eNodeB will be followed.<br>
<img src="Option3.png" alt="NSA vs SA Overview" width="400"/></li>
<li><b>Option 4:</b> Main network is 5GC and dual connectivity is there <br>
Option 4: 5GC is connected with gNodeB and gNodeB shares the required data with eNodeB<br>
Option 4a: eNodeB and gNodeB are both directly connected with 5GC.<br>
Option 4x: it is not a very likely option.<br>
<img src="Option4.png" alt="NSA vs SA Overview" width="400"/>
</li>
<li><b>Option 5:</b> The main network is 5GC, but device has access to LTE only, so the LTE is upgraded to understand the protocols of 5GC and then its called eLTE (e stands for enhanced)<br>
<img src="Option5.png" alt="NSA vs SA Overview" width="400"/></li>
<li><b>Option 6:</b> Here the network is 4GC, but device has access to gNodeB only (it is not supported)<br>
<img src="Option6.png" alt="NSA vs SA Overview" width="400"/></li>
<li><b>Option 7 (NG-EN-DC):</b> It is same as option 4 but the master access technology is eNodeB and secondary is gNodeB, this was the reason of the inexistence of Option 4x
<br>
<img src="Option7.png" alt="NSA vs SA Overview" width="400"/></li>
</ol>
</li> 
</ul>

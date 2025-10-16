
  <h1 align="center">O-RAN </h1>

  <h2>1. Service Management and Orchestration (SMO)</h2>
  <p><strong>SMO</strong>  is responsible for orchestration, automation, and analytics of RAN components.</p>

  <h3>Key Functions:</h3>
  <ul>
    <li> Defines, provisions, and manages end-to-end services.</li>
    <li> Deploys and scales VNFs on the O-Cloud.</li>
    <li> Implements AI/ML-driven closed-loop optimization.</li>
    <li>Collects measuring data for RICs and AI/ML models.</li>
  </ul>

  <h2>2. RAN Intelligent Controller (RIC)</h2>
  <p>The <strong>RIC</strong> introduces intelligence and programmability into the RAN using AI/ML. It is divided into two types:</p>

  <h3>(a) Non-Real-Time RIC (Non-RT RIC)</h3>
  <ul>
    <li>Operates on timescales greater than 1 second.</li>
    <li>Part of the SMO layer.</li>
    <li>Handles policy management, AI model training, and long-term analytics.</li>
    <li>Communicates with Near-RT RIC via the <strong>A1 interface</strong>.</li>
  </ul>

  <h3>(b) Near-Real-Time RIC (Near-RT RIC)</h3>
  <ul>
    <li>Operates between 10 milliseconds to 1 second.</li>
    <li>It can observe, analyze, and change how the RAN (Radio Access Network) operates almost immediately</li>
    <li>Uses <strong>xApps</strong> for specific functions (handover, interference, load balancing).</li>
    <li>Connects to RAN nodes through the <strong>E2 interface</strong>.</li>
  </ul>

  <h2>3. O-RAN Interfaces</h2>
  <h3>O1 Interface</h3>
  <p>Connects the SMO with O-RAN nodes (O-CU, O-DU, O-RU). Used for configuration, fault, and performance management using <strong>NETCONF/RESTCONF</strong> and <strong>YANG</strong> models.</p>
  <strong>NETCONF</strong>- NETCONF is a standard protocol used by the SMO to send configuration commands and retrieve data from O-RAN nodes (like O-CU, O-DU, O-RU).Uses XML and operates on SSH<br><br>
  <strong>RESTCONF</strong>- RESTCONF is a RESTful API-based alternative to NETCONF, It performs the same tasks, but uses HTTP/HTTPS instead of SSH and JSON/XML instead of XML only.
  <br><br>
  <strong>YANG models</strong>- YANG is a data modeling language that defines how network data is structured — both configuration (what can be changed) and state (what’s currently happening).<br>Defines what parameters a device supports (frequency, power, status, etc.).

Ensures consistency between devices from different vendors.<br> Used by NETCONF and RESTCONF to understand the data’s structure.
<br><br>
<i><b>(YANG defines what data and configuration option exists, NETCONF configures and retrieves the data using XML and SSH, RESTCONF does the same but uses HTTP and JSON/XML)</b></i>

  <h3>A1 Interface</h3>
  <p>Connects Non-RT RIC and Near-RT RIC. Used to exchange policies, ML models, and enrichment information.</p><br>
  Enrichment information means contextual data provided by the Non-RT RIC to the Near-RT RIC to improve decision-making.


Examples:

Predicted user mobility or traffic demand patterns.

External data like weather, time of day, or special events.

Historical performance analytics.

  <h3>E2 Interface</h3>
  <p>Connects Near-RT RIC with RAN nodes (O-DU, O-CU). Enables near real-time control and optimization using the <strong>E2 Application Protocol (E2AP)</strong>.</p><br>
  E2AP is the control protocol used over the E2 interface between the Near-RT RIC and RAN nodes (O-DU/O-CU).
  
  It defines how the RIC sends and receives:


Control messages (to adjust RAN behavior in real time), and

 Reports/indications (performance, status, events) from RAN nodes.

  <h2>4. OAM (Operations, Administration, and Maintenance)</h2>
  <ul>
    <li> Daily management of network functions.</li>
    <li>User roles, provisioning, and access control.</li>
    <li> Fault management, updates, and system health.
    
    System health refers to the overall status and performance of a system, including resource usage, uptime, error rates, and responsiveness, to ensure reliable operation.</li>
  </ul>


  <h2>6. O-Cloud (Open Cloud Infrastructure)</h2>
  <p><strong>O-Cloud</strong> provides the compute, storage, and network infrastructure for O-RAN components. It supports both VNFs and CNFs and is managed via the <strong>O2 interface</strong> by the SMO.</p>

  <h2>7. VNFs and CNFs</h2>
  <ul>
    <li><strong>VNF (Virtual Network Function):</strong> Runs in Virtual Machines (VMs) using hypervisors like KVM or VMware.</li>
    <li><strong>CNF (Cloud-Native Network Function):</strong> Runs as containers orchestrated by Kubernetes.</li>
  </ul>

  
 
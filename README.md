<h1>Wazuh SIEM Active Response</h1>

<h2>Description</h2>
In this project, I implemented and configured the open-source SIEM solution Wazuh to collect and monitor logs within my homelab environment. I will demonstrate the setup of active-response, a Wazuh feature that dynamically blocks threat actors based on the associated rule_id of their malicious actions.

For this example, I configured the system to drop SSHd login attempts, identified by rule_id 5710, using the firewall drop rule command. Additionally, I integrated Slack notifications to provide real-time alerts for these security events.

<br />


<h2>Languages and Utilities Used</h2>

- <b>Widows CMD</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> 
- <b>Linode Cloud</b>
- <b>Wazuh</b>

<h2>Program walk-through:</h2>

<p align="center">
SSH-5710 Event: threat actor attempts to SSH into server. <br/>
<img src="https://i.ibb.co/HxKdvMv/SSH-5710.jpg"  alt="SSH-Event" height="80%" width="80%">
<br />
<br />
Active response rule: rule configured in the OSSEC file.  <br/>
<img src="https://i.ibb.co/0sHHTLK/Active-response-rule.jpg" height="80%" width="80%" alt="Active-response-rule"/>
<br />
<br />
Event-triggered active response rule: The firewall is triggered and the threat actor is dropped.  <br/>
<img src="https://i.ibb.co/zh2P8pd/triggered-active-response.jpg" height="80%" width="80%" alt="Event-triggered"/>
<br />
<br />
Slack notification:  <br/>
<img src="https://i.ibb.co/BZK8whf/Slack-integration.jpg" height="80%" width="80%" alt="Slack"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

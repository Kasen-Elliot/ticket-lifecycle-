<p align="center">
<img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/0982bc11-b359-40f8-a166-330cf78c5d40" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle Examples</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. This tutorial assumes you have completed both the <a href= ""> installation </a> and <a href = "">configuration</a> of osTicket

</br>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
  <li>osTicket</li>
</ul>

</br>

<h2>Operating Systems Used </h2>
<ul>
  <li>Windows 10</li>
</ul>

</br>

<h2>Ticket Lifecycle Stages</h2>
<ol>
  <li>Intake</li>
  <li>Assignment & Communication</li>
  <li>Working the Issue</li>
  <li>Resolution</li>
</ol>

</br>

<h2>Lifecycle Stages</h2>



<h3>Intake</h3>

<p>
  <ul>
    <li>From the <b>End User's</b> side (Karen Karen), they create a ticket through osTicket's <a href = "http://localhost/osTicket/ ">local host site</a> and fill their information, select a Help Topic</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/d3cd4aa2-7713-4990-8fdb-921ffd356f33" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The End User then writes ticket through the <b>Issue Summary</b> and adds a subject and details of the ticket much similar to writing an email</li>
    <ul>
      <li>In this example, Karen creates the ticket under the Help Topic of a Business Critcal Outage (made from our configuration of osTicket) explaining the mobile banking application is suffering a 404 error</li>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/6a6f9eb5-f3a8-4cb4-9ae1-9184a5f0f65c" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Karen then creates the ticket and is sent to <b>Agent</b> Jane Doe (which we've set as Supreme Admin is able to see all incoming tickets in the configuration tutorial) who views it from the <a href = "http://localhost/osTicket/scp/login.php">local help desk login</a></li>
    <ul>
      <li><b>Note</b>: Priorities have not been set for other incoming tickets such as ticket #951342 where end user Ken is requesting an upgrade to Adobe Reader. SLA plans need to be set for these tickets hence why they are all under the priority state of "Normal"</li>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/a8480942-0df2-4c28-b7a1-b4aa93151731" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<h3>Assignment & Communication</h3>

<p>
  <ul>
    <li>The Business Critical Outage ticket by Karen numbered 282733 is assigned to the Agent Jane Doe. From Jane's perspective, this is how the ticket first looks.</li>
    <ul>
      <li>The Agent is able to message the End User through the <b>Ticket Thread</b> located in the bottom of the ticket page</li>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/877993e0-d217-4a6a-9232-6bec56e6941f" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>By going to the link next to <b>Priority</b>, you are able to set the priority of the ticket to Low, Normal, High, or Emergency</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/c8a2c8ce-4e3a-42f7-8bc0-54591d784ac4" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>By going to the greyed out link --Unassigned-- next to <b>Assigned to</b>, you can assign the ticket to a Team or Agents. Note if we were to assign it to an Agent outside of Agent Jane's Department, it will not appear in their feed.</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/18c672b4-d7e6-4ad3-80db-bd52e54c130e" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>By going to the link next to <b>SLA Plan</b> to set the SLA Plan from Default SLA to one our SLA Plans we have created in configuration. For this Business Critical Outage ticket, it'll be set to SEV-A</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/06f40b6e-d411-4b2d-9d37-2e01596f8a86" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>By going to the link next to <b>Department</b> to set the Department. For this Business Critical Outage ticket, it'll be set from Support to System Administrators</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/318eca83-9f44-48df-a7a9-8b1b50037390" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The Ticket Thread is updated when we make the changes to ticket</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/a0342735-ac49-498d-9c35-8bbc99d3b455" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The Agent can message the End User through the Ticket Thread to update the User on the ticket as well as set the status of the ticket (which is left as <b>Open</b> since we need to work it out)</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/991ab730-bc53-4429-bb7c-821397bedbcf" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<br />

<h3>Working the Issue and Resolution</h3>

<p>
  <ul>
    <li>Following from our Assignment of Departments and Communication with the End User, the issue in our hypothetical Critical Banking Outage ticket has been resolved thanks to System Engineering. The Agent should now communicate the issue with the End User using the Ticket Thread and set the status of the ticket from Open to <b>Resolved</b>. Upon posting the Reply, the ticket is <b>Closed</b>.</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/585f115a-193d-4dbf-9a46-871627583faf" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Closed tickets can be found under the Closed section in our Tickets tab, where information and status of the tickets are archived. It is good practice for Agents to study Closed tickets to improve their experience in working with them</li>
    <ul>
      <li><img src="https://github.com/Kasen-Elliot/ticket-lifecycle-/assets/127895952/d8aed5cc-8d8d-436a-9c1b-efe4d93bc931" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<br />

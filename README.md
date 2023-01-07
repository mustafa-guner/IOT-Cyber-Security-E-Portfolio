<img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b8/EMU_Cyprus.svg/1200px-EMU_Cyprus.svg.png" width="200" height="200"> <a href="https://www.emu.edu.tr/en"><h1>Eastern Mediterranean University</h1></a>

<h2>IOT & Cyber Security - ITEC 442 Course</h2>

**🎯Motivation**: The aim of the project is, to create E-Portfolio for the lab work we prepare week by week. Each week has its own articles and report. You can review all articles and exercises week by week. Some of them may include external links for blog posts. You can check and get more information.

<h2>Week 1-2</h2>

<h3>Week 1</h3>
Week one was all about <b>Digitalization and Energy Crisis in 2022</b>. We have an article written by 3 authors about the security implications of the digital economy. Week 1 basically all about finding answers to the following questions:

- What is the definition of a fully digital enterprise?
- What are the cyber-security challenges/concerns with a fully digital enterprise?
- What are the cyber security challenges for bricks and mortar SMEs wanting to become digital enterprises?

I read the article and found external references for answering those questions properly. You can find the reference links down below the word document.

<h3>Week 2</h3>
Week two was all about <b>Scanning Activity</b> which means we used some CMD commands to check following tasks:
  
- <b>How many hops do we have from our machine to target website?</b>
   <code>tracert [target website link]</code>

- <b>Which step causes the biggest delay in the route?</b>
  <code>tracert [target website link]</code>

- <b>What is the average duration of that delay?</b>
  <code>ping [target website link]</code>

- <b>Checking main nameservers for the target website</b>
  <code>nslookup [target website link]</code>

- <b>Details of the MX Record for the target website</b>

  1. <code>nslookup</code>
  2. <code>set q=MX</code>
  3. <code>[target website link]</code>

- <b>Who is the registered contract? </b>
  <code>whois [target website address]</code>

- <b>Find out where the target website is hosted.</b>
  <code>nslookup [target website link]</code>

<p>Also, i have a reflection section at end of the word document to express my observations and feelings about the task.</p>
<p>I faced an issue while I was trying to check the MX record for the target website. I was not able to check MX records via the command line. 
  Since I have been using ubuntu for almost 1 year I decided to use ubuntu for this task instead of LINUX. 
  I found useful documentation on <a href="https://www.cloudflare.com/learning/dns/dns-records/dns-mx-record/">cloudflare.com</a> and I executed the following code.
  First, I entered <code>nslookup</code> command then set a filter to only collect MX records and related information (<code>q=MX</code>) and added the target website.
  At the end I was able to check MX records and SMTP email address of the target website.</p>
<p>At the end of the week 2 we have also some end of unit activitiy questions.The questions and summariezed answers are the followings.</p>
<ul>
<li>
<h3>Activity 1</h3>
<p><strong>Question:</strong> Cloud platforms are becoming a very common commodity in the digital system. What are the benefits and draw backs in Cloud solutions with respect to cyber security? Present an argument with minimum 500 words in favour of or against cloud storage. What are the security risks involved in cloud vs local store . You should post your solution in the discussion group and provide at least two references</p>
<p><strong>Answer:</strong> Cloud storage solutions offer scalability, cost-effectiveness, automatic updates, and data backup and recovery, but also have drawbacks such as dependence on internet connection, security concerns, limited control, limited customization, vendor lock-in, and security risks. Local storage has the risk of physical damage or theft and is vulnerable to natural disasters, but also offers more control. Businesses must weigh the benefits and drawbacks and consider their specific needs when deciding between cloud and local storage for cyber security.</p>
</li>

<li>
<h3>Activity 2</h3>
<p><strong>Question:</strong> In 2017 a ransomware termed as WannaCry unleased its malicious attack on a global scale. What cautions and safeguards should have been in place that could have averted this attack?</p>
<p><strong>Answer:</strong> The WannaCry ransomware attack in 2017 exploited a vulnerability in older versions of Windows and encrypted users' data. To prevent similar attacks, it is important to keep software and operating systems up to date, use antivirus software, implement a firewall, use strong passwords, regularly back up data, educate employees about cyber security, and use multi-factor authentication.</p>
</li>

<li>
<h3>Activity 3</h3>
<p><strong>Question:</strong>Why is it important to have a backup system in place that works closely with cyber security framework? How are these two components are related? Please use your own personal computer as hypothetical machine and list the steps that you will adopt to backup your data.</p>
<p><strong>Answer:</strong> Having a backup system in place is important for protecting against data loss due to cyber attacks, hardware failures, or other disasters. To create a backup system for a personal computer, identify the data that needs to be backed up, choose a backup method, set up a schedule for backups, test the system to ensure it is working properly, and store the backup in a secure location. This will create a backup system that works closely with the cyber security framework to protect against data loss.</p>
</li>
</ul>

<h2>Week 3-4</h2>
<p>On week 3 and 4 we discussed Cyber Kill Chain. Understanding the Cyber Kill Chain can help organizations to develop defenses at each stage of an attack and to implement effective cybersecurity measures to reduce the risk of a successful attack.
</p>  
<p>Understanding the Cyber Kill Chain can help organizations to develop defenses at each stage of an attack and to implement effective cybersecurity measures to reduce the risk of a successful attack.</p>
<table>
<thead>
<tr>
  <th>Phase</th>
  <th>Description</th>
  <th>SolarWinds Exploit</th>
  <th>Mitigations</th>
</tr>
</thead>
<tbody>
  <tr>
    <td>
      Reconnaissance
    </td>
     <td>
     The attacker gathers information about the target to plan the attack.
    </td>
    <td>
      It is not clear at this time how the attacker obtained information about SolarWinds and its
                    customers
    </td>
    <td>
      <ul>
        <li>Implement access controls to limit the information that is available to potential attackers. </li>
        <li>Monitor network activity and look for signs of reconnaissance. </li>
        <li>Use threat intelligence to stay informed about potential threats and the tactics, techniques, and procedures (TTPs) used by attackers.</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
      Weaponization
    </td>
     <td>
     The attacker creates a tool or payload to deliver the attack.
    </td>
    <td>
     The attacker created a malicious update for the SolarWinds Orion software, which was then
                    distributed to customers through the normal update process.
    </td>
     <td>
      <ul>
        <li>Implement code signing to verify the authenticity of software updates.</li>
        <li>Use multi-factor authentication for update servers and processes. </li>
        <li>Use a secure supply chain to ensure that software is not tampered with during the development and distribution process.</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
      Delivery
    </td>
     <td>
     The attacker delivers the weapon to the target.
    </td>
    <td>
     The attacker delivered the malicious update to SolarWinds customers through the normal update
                    process.
    </td>
     <td>
      <ul>
        <li>Use network segmentation to isolate systems and limit the spread of an attack.</li>
        <li>Monitor network activity and look for signs of unusual or unauthorized traffic. </li>
        <li>Monitor network activity and look for signs of unusual or unauthorized traffic.</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
      Exploitation
    </td>
     <td>
     The attacker exploits a vulnerability in the target system.
    </td>
    <td>
      The attacker exploited a vulnerability in the SolarWinds Orion software to gain access to the
                    systems of customers who installed the malicious update.
    </td>
     <td>
      <ul>
        <li>Regularly apply security patches and updates to systems to fix vulnerabilities. </li>
        <li>Use vulnerability management to identify and address vulnerabilities in a timely manner.  </li>
        <li>Use firewalls and other security controls to block access to known vulnerabilities</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
      Installation
    </td>
     <td>
     The attacker installs the payload on the target system.
    </td>
    <td>
      The attacker installed a backdoor on the systems of customers who installed the malicious update.
    </td>
     <td>
      <ul>
        <li>Implement endpoint security to protect against the installation of malicious software.  </li>
        <li>Monitor system activity to detect the installation of unauthorized software. </li>
        <li>Use application whitelisting to allow only trusted applications to run on systems. This can prevent malware from being installed or executed.</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
        Command and control
    </td>
     <td>
      The attacker establishes a connection to the payload and gains control of the target system.
    </td>
    <td>
      The attacker established a connection to the backdoor on the compromised systems and gained control
                    of them.
    </td>
     <td>
      <ul>
        <li>Implement network segmentation and access controls to limit the ability of attackers to communicate with compromised systems. </li>
        <li>Monitor network activity and look for signs of C2 traffic, such as outbound connections to known C2 servers or unusual traffic patterns. </li>
        <li>Use threat intelligence to stay informed about known C2 servers and tactics used by attackers..</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td>
         Actions on objectives
    </td>
     <td>
      The attacker performs their desired actions on the target system.
    </td>
    <td>
       The attacker used the compromised systems to access other networks and gather information.
    </td>
     <td>
      <ul>
        <li>Regularly back up data to enable the restoration of affected systems and data.</li>
        <li>Use incident response plans and processes to identify the objectives of an attack and take appropriate action to prevent or mitigate them </li>
        <li>Monitor system activity for signs of unauthorized actions, such as data exfiltration or the modification of critical files.</li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

<p><strong>Tools used to utilize in each phase:</strong></p>
<ol>
  <li>
    <p><strong>Reconnaissance phase: </strong></p>
    <ul>
      <li>
        <p><strong>Access control systems: </strong>
        These systems can limit the information that is available to potential attackers.
        </p>
      </li>
      <li>
        <p>
        <strong>Network monitoring tools:  </strong>
     These tools can detect signs of reconnaissance activity, such as scans or probes of a network.
        </p>
      </li>
      <li>
        <p>
        <strong>Threat intelligence platforms: </strong>
          These platforms provide information about potential threats and the tactics, techniques, and procedures (TTPs) used by attackers
        </p>
      </li>
    </ul>
  </li>

  <li>
    <p><strong>Weaponization phase: </strong></p>
    <ul>
      <li>
        <p><strong>Code signing tools: </strong>
        These tools verify the authenticity of software updates and can prevent the distribution of malicious updates.
        </p>
      </li>
      <li>
        <p>
        <strong>Multi-factor authentication systems:  </strong>
      These systems can be used to secure update servers and processes, making it more difficult for attackers to deliver malware.
        </p>
      </li>
      <li>
        <p>
        <strong>Supply chain management tools: </strong>
        These tools can help ensure that software is not tampered with during the development and distribution process.
        </p>
      </li>
    </ul>
  </li>

  <li>
    <p><strong>Delivery phase: </strong></p>
    <ul>
      <li>
        <p><strong>Network segmentation tools: </strong>
       These tools can isolate systems and limit the spread of an attack.
        </p>
      </li>
      <li>
        <p>
        <strong>Network monitoring tools:  </strong>
     These tools can detect unusual or unauthorized traffic that could indicate an attack.
        </p>
      </li>
      <li>
        <p>
        <strong>Email filtering tools: </strong>
        These tools can prevent the delivery of malicious emails by blocking or quarantining suspicious messages.
        </p>
      </li>
    </ul>
  </li>
    <li>
    <p><strong>Exploitation phase: </strong></p>
    <ul>
      <li>
        <p>
        <strong>Vulnerability management tools: </strong>
       These tools can help identify and address vulnerabilities in a timely manner, reducing the risk of exploitation.
        </p>
      </li>
      <li>
        <p>
        <strong>Firewall systems:  </strong>
    These systems can block access to known vulnerabilities, helping to prevent exploitation.
        </p>
      </li>
    </ul>
  </li>

   <li>
    <p><strong>Installation phase: </strong></p>
    <ul>
      <li>
        <p>
        <strong>Endpoint security tools: </strong>
     These tools can detect and block malware from being installed on systems.
        </p>
      </li>
      <li>
        <p>
        <strong>System monitoring tools: </strong>
    These tools can alert administrators to unusual activity that could indicate an attempt to install malware.
        </p>
      </li>
       <li>
        <p>
        <strong>Application whitelisting tools: </strong>
    These tools allow only trusted applications to run on systems, which can prevent malware from being installed or executed.
        </p>
      </li>
    </ul>
  </li>

   <li>
    <p><strong>Command and Control (C2) phase: </strong></p>
    <ul>
      <li>
        <p>
        <strong>Network monitoring tools: </strong>
   These tools can help detect C2 traffic, such as outbound connections to known C2 servers or unusual traffic patterns.
        </p>
      </li>
      <li>
        <p>
        <strong>Threat intelligence platforms: </strong>
   These platforms provide information about known C2 servers and tactics used by attackers.
        </p>
      </li>
       <li>
        <p>
        <strong>Firewall systems: </strong>
   These systems can block access to known C2 servers.
        </p>
      </li>
    </ul>
  </li>

   <li>
    <p><strong>Actions on Objectives phase: </strong></p>
    <ul>
      <li>
        <p>
        <strong>Data backup tools: </strong>
     These tools enable the restoration of affected systems and data.
        </p>
      </li>
      <li>
        <p>
        <strong>Data loss prevention (DLP) systems: </strong>
   These systems detect and prevent the exfiltration of sensitive data.
        </p>
      </li>
       <li>
        <p>
        <strong>Access control systems: </strong>
   These systems limit the ability of unauthorized users to access and modify critical systems and data.
        </p>
      </li>
    </ul>
  </li>
</ol>

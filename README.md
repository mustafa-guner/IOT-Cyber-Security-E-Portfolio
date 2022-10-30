<img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b8/EMU_Cyprus.svg/1200px-EMU_Cyprus.svg.png" width="200" height="200"> <a href="https://www.emu.edu.tr/en"><h1>Eastern Mediterranean University</h1></a>

<h2>IOT & Cyber Security - ITEC 442 Course</h2>

**🎯Motivation**: The aim of the project is, to create E-Portfolio for the lab work we prepare week by week. Each week has its own articles and report. You can review all articles and exercises week by week. Some of them may include external links for blog posts. You can check and get more information.

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
  At the end I was able to check MX records and SMTP email address of the target website.<p>

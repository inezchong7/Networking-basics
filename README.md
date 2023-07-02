<h1>Nmap (Network Mapper)</h1> 

<h2>Description</h2>
<p>My notes about Networking are documented here.</p>

<h2>📝Notes</h2>
<h4><u>OSI (Open Systems Interconnection) Model:</u></h4>
<p><b></b> A standardised model used to demonstrate computer networking theory. The 7 layers are - </p>
<ol>
  <li><b>Application</b>: provides networking options to programs running on a computer</li>
  <li><b>Presentation</b>: receives data from Application layer, then translates the data into a standardised format </li>
  <li><b>Session</b>: receives correctly formatted data from Presentation layer; establishes and maintains connection with other computers; allows multiple requests to different endpoints simultaneously (like opening a few tabs in a web browser)</li>
  <li><b>Transport</b>: chooses a protocol to transmit the data (eg. <b>TCP , UDP </b>) </li>
<p>**TCP/ Transmission Control Protocol = reliable transmission; constant communication; data/ segments sent to all the right places at acceptable speed; for file transfers.</p>
<p>**UDP/ User Datagram Protocol = data/ datagrams thrown at receiving computer; for video streaming (eg. pixelated Skype video durig bad connection) </p>
  <li><b>Network:</b>locates the request destination through Logical addressing (eg. locating IP addresses in IPV4 format)</li>
  <li><b>Data Link:</b>checks for corruption in the received data; adds MAC address to the data for physical end-destination; data formatted for transmission.</li>
  <p>**MAC/ Media Access Controls are found with each computer's NIC/ Network Interface Card.</p>
  <li><b>Physical:</b>converts binary data into signals to send; converts incoming signals into binary data to receive.</li>
</ol>
<img src=""> 

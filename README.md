<h1>Networking basics</h1> 

<h2>Description</h2>
<p>My notes about Networking are documented here.</p>

<h2>📝Notes</h2>
<h4><u>➡️OSI (Open Systems Interconnection) Model:</u></h4>
<p><b></b> A standardised model used to demonstrate computer networking theory. The 7 layers are - </p>
<ul>
  <li><b>Application (7)</b>: provides networking options to programs running on a computer</li>
  <li><b>Presentation (6)</b>: receives data from Application layer, then translates the data into a standardised format </li>
  <li><b>Session (5)</b>: receives correctly formatted data from Presentation layer; establishes and maintains connection with other computers; allows multiple requests to different endpoints simultaneously (like opening a few tabs in a web browser)</li>
  <li><b>Transport (4)</b>: chooses a protocol to transmit the data (eg. <b>TCP , UDP </b>) </li>
<p>**TCP/ Transmission Control Protocol = reliable transmission; constant communication; data/ segments sent to all the right places at acceptable speed; for file transfers.</p>
<p>**UDP/ User Datagram Protocol = data/ datagrams thrown at receiving computer; for video streaming (eg. pixelated Skype video durig bad connection) </p>
  <li><b>Network (3):</b>locates the request destination through Logical addressing (eg. locating IP addresses in IPV4 format)</li>
  <li><b>Data Link (2):</b>checks for corruption in the received data; adds MAC address to the data for physical end-destination; data formatted for transmission.</li>
  <p>**MAC/ Media Access Controls are found with each computer's NIC/ Network Interface Card.</p>
  <li><b>Physical (1):</b>converts binary data into signals to send; converts incoming signals into binary data to receive.</li>
</ul>

<img src="https://github.com/inezchong7/Networking-basics/assets/106855786/e854fc88-09c9-45b4-92cd-6e05fc89a55e"> 

<h4>➡️Encapsulation</h4>
<p> The process by which data is modified at every layer and sent from one computer to another. (includes layers 7 to 1) </p>
<p>**Data has different names at different layers.</p>
<ul>
  <li>At layers 7, 6, 5: data = data</li>
  <li>At layer 4: data = segment (TPC) or datagram (UDP) </li>
  <li>At layer 3: data = packet</li>
  <li>At layer 2: data = frame</li>
  <li>At layer 1: data = bits</li>
</ul>
<p>De-encapsulation is the stripping of data at each layer upon receival. </p>

<img src="https://github.com/inezchong7/Networking-basics/assets/106855786/4dbac88d-2ce2-411b-b457-e58500e7bca0">

<h4>➡️TCP/ IP model</h4>
<p>Firstly, connection must be established. This is done through the <b>3-way handshake</b>.</p>
<p>The 3-way handshake: SYN (=synchronize; connection request) - SYN/ACK (server response) - ACK (=acknowledgement; connection confirmation)</p>
<img src="https://github.com/inezchong7/Networking-basics/assets/106855786/33b864d4-197c-43ea-a592-b910c671bc09">

The 4 layers of networking:
<ul>
  <li><b>Application</b>>: </li>
  <li><b>Transport</b>:</li>
  <li><b>Internet:</b></li>
  <li><b>Network Interface:</b></li>
</ul>

<p>**A header is added during encapsulation, and removed during de-encapsulation, same as in OSI.</p>
<img src="https://github.com/inezchong7/Networking-basics/assets/106855786/d590b8d1-713d-433a-8af6-be26eada8669">

<h4>➡️DNS requests</h4>
<p> When a request to a website is made, computer checks local cache for IP address first. If not found, request is sent to a recursive DNS server. Is still not found, requests is passed to Root Name Server. Root Name Servers pass the request down to appropriate TLD/ Top-Level Domain servers (low-levels). TLDs are categorized by extensions (eg. .com, .co). Next-level down is Authorative Name servers. All DNS records are directly stored in Authorative Name servers. /p>


Week 6 – Networking and Cyber Security

Topic: Internet Applications
Goal: Build and analyze web applications, capture network packets, and understand HTTP communication.

Task 1 – Knowledge Test 

Helps assess my understanding before starting practical activities.

Task 2 – Create Web Pages in OpenWRT 

Access my web server at http://192.168.56.2/

Files are stored in /srv/www
Steps:

Copy index.html to a new file (your student ID).

Add a hyperlink in index.html to your new page.

Edit my new HTML page to:

Add my name and ID.

Show current date/time when a button is clicked.

Use a custom CSS file.

Create a CSS file to style my page (e.g., change text color).
Upload to journal:

index.html, yourID.html, mystyle.css

Screenshot after clicking “Show date and time.”

Task 3 – Capture HTTP Packets 

On OpenWRT, run tcpdump to capture HTTP traffiq.

Perform the following in your Windows browser:
a) Visit my OpenWRT web page.
b) Click the new HTML link.
c) Press the “Show date and time” button twice.

Stop the capture using Ctrl + C.

View my ARP Table in PowerShell to identify reachable devices.

In my journal:

HTTP packet capture (.pcap)

Screenshot or text of ARP Table

Task 4 – Analyse HTTP Packet Capture

Open the .pcap file in Wireshark and filter for HTTP.
Analyse:
a) Explain each HTTP request and response (trigger, request, and result).
b) List 5 addressing values for host, transport, and application layers.
c) Determine if the “Show date/time” button sent a server request.
d) Draw a packet diagram of one HTTP request (include sizes and addresses).
e) Identify the referrer and its role for web servers.
f) Note what the server learns about your browser.
g) Identify the HTTP version and transport protocol.
h) Find packets showing connection setup (TCP 3-way handshake).
i) Identify acknowledgment packets and when they’re sent.

In my journal:

Written answers (a–i) with packet details.

PNG and .drawio file of the HTTP packet diagram.

Task 5 – View my Cookies 

Open browser developer tools → view cookies for a site you visit often.

Note what information cookies store (e.g., login, session, preferences).

Don’t include personal values — describe the types of data stored.

In my journal:

Explanation of cookie data types stored by websites.

Slide 7: Summary

Built a simple website using HTML, CSS, and JavaScript in OpenWRT.

Captured and analyzed HTTP traffic using Wireshark.

Learned how HTTP requests, responses, and cookies work.

Observed how ARP tables and TCP connections support web communication.

Strengthened web development and network analysis skills.

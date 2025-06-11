# cs39006-assignment-1--using-wireshark-udp-sockets-solved
**TO GET THIS SOLUTION VISIT:** [CS39006 Assignment 1- Using Wireshark, UDP sockets Solved](https://mantutor.com/product/cs39006-solved-2/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114014&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS39006 Assignment 1- Using Wireshark, UDP sockets Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

PART A: Exploring Packet Sniffer and Packet Analyzer

The objective of this part of the assignment is to understand the network packet structures and different fields present at the packet headers corresponding to different layers of the protocol stack. For this assignment, you need to install Wireshark on your machine and keep your machine connected with the Internet.

To start with, execute the following steps.

1) Ensure that no browsing activity is going on in your machine. Close all the browser tabs.

2) Download and run Wireshark.

3) Start capturing packets over your default (active) network interface.

4) Open a browser tab and open the website http://iitkgp.ac.in/. 5) Wait for 1 minutes.

6) Now on the same browser tab, open the website https://www.cornell.edu/.

7) Close the browser tabs.

8) Stop packet capture.

9) Save the pcap file from Wireshark.

Now answer the following questions by analyzing the packet traces. Do not use any other tools other than wireshark, use its features to answer the questions to learn them better.

1. How many packets do you see for the following protocols?

a. TCP and UDP together

b. IPv4 and IPv6?

2. What is the total amount of data being received for the following two cases?

a. When you access http://iitkgp.ac.in

b. When you access https://www.cornell.edu

3. How many DNS packets have you observed in total?

a. Create a &lt;Domain Name, IP&gt; table by exploring the queries and the answers in those DNS packets. The Domain Name will be the domain for which you see a query, and the IP address will be the address that is being returned against the corresponding query.

b. Can you find out the IP of the DNS servers by exploring the DNS packets?

4. Answer the following when you access the site http://iitkgp.ac.in.

a. How many HTTP GET requests do you observe? List down the GET requests.

b. For each of the HTTP GET requests you see above, find out (ii) the total number of TCP segments being received, and (ii) the total amount of data being received in the corresponding HTTP Response message.

Submission Instructions:

Upload the pcap file that you have used in a password-less shareable Google drive folder (do not upload the file directly in moodle). Create a doc file named &lt;roll_number&gt;_Assignment1_A.doc (replace &lt;roll_number&gt; with your roll number) with your answers. The header of the doc file should be as follows.

=====================================

Assignment 1 (Part A) Submission

Name: &lt;Your_Name&gt;

Roll number: &lt;Your_Roll_Number&gt;

Link of the pcap file: &lt;Google_Drive_Link_of_the_pcap_File&gt; =====================================

PART B: Simple Datagram Socket using POSIX C

The objective of this assignment is to get familiar with datagram sockets using POSIX C

programming. The target is to establish a communication between two computers (processes) using a datagram socket. A datagram socket uses a simple communication paradigm to transfer short messages between two computers (processes) without ensuring any reliability.

Your task will be to write two programs – one program corresponding to the server process and another program corresponding to the client process. The client process requests for the content of a file (by providing the file name) and the server process sends the contents of that file to the client.

For simplicity, we assume that the file is a simple text file that contains a set of words, with the first work being HELLO and the last word being END. We assume that HELLO and END are two special keywords that do not come anywhere except at the first line (HELLO) and at the last line (END). The content of a sample file looks as follows.

HELLO

SOCKET PROGRAMMING

COMPUTER

NETWORK

TCP UDP END

The transfer of the contents of the file works using a communication protocol as follows.

1. The client first sends the file name to the server (assume the name has les than 100 characters).

2. The server looks for the file in the local directory, if the file is not there it sends back with a message NOTFOUND &lt;FILENAME&gt;, where &lt;FILENAME&gt; is the name of the file requested by the client. By receiving this message, the client prints an error message “File &lt;FILENAME&gt; Not Found” and exits.

3. If the file is present, the server reads the first line of the file, which contains HELLO, and sends this message to the client.

4. After receiving HELLO, the client creates a local file (a different file name from the requested one) and sends a message WORD1 to the server. This message indicates that the client is requesting for the first word.

5. After receiving the message WORD1, the server sends the first word (after HELLO) to the client. The client writes this word to the local file after receiving it and sends the message WORD2 to request for the next word. This procedure continues for each word.

6. On receiving WORDi, the server sends the i-th word to the client. This process continues until the client receives the keyword END.

7. Once the client receives the keyword END, it closes the local file after writing the last word to the file.

Is this a good file transfer protocol?

Submission Instruction:

You should write two C programs – wordserver.c (contains the server program) and wordclient.c (contains the client program). Keep these two files in a single compressed folder (zip or tar.gz) having the name &lt;roll number&gt;_Assignment1_B.zip or &lt;roll number&gt;_Assignment1_B.tar.gz.

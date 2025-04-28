# cmsc440-assignment-1--simple-ping-application-solved
**TO GET THIS SOLUTION VISIT:** [CMSC440 Assignment 1- Simple PING Application Solved](https://www.ankitcodinghub.com/product/cmsc-440-programming-assignment-simple-ping-application-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119160&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMSC440  Assignment 1-  Simple PING Application Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Description:

The goal of this assignment is to allow you to demonstrate your knowledge of socket programming for UDP connections. You will learn how to send and receive datagram packets using UDP sockets and, how to set a proper socket timeout. Throughout this assignment, you will gain familiarity with a Ping application and its usefulness in computing statistics such as packet loss rate. In this assignment, you will develop a simple Internet ping server written, and implement a corresponding client. The functionality provided by these programs is similar to the functionality provided by standard ping programs available in modern operating systems. However, these programs use a simpler protocol, UDP, rather than the standard Internet Control Message Protocol (ICMP) to communicate with each other. The ping protocol allows a client machine to send a packet of data to a remote machine, and have the remote machine return the data back to the client unchanged (an action referred to as echoing). Among other uses, the ping protocol allows hosts to determine round-trip times to other machines.

PINGClient

• Your client should be named PINGClient.java, PINGClient.py, PINGClient.c, etc.

• Your ping client should be able to send ping and receive responses from your ping server.

• Your client should accept a two command-line argument: the first one is either the hostname or the IP of your ping server, and the second is the port number your server is running at.

o Example: PINGClient egr-v-cmsc440-2.rams.adp.vcu.edu 10500 o Or: PINGClient 10.0.0.2 10500

o If any of the arguments are incorrect, exit after printing an error message of the form “ERR – arg x”, where x is the argument number.

• Your ping client should send ping packets to the ping server given in the hostname/IP and the port thru a UDP connection. o Handle exceptions as you wish — for example, if the host doesn’t exist or the port given is not open

• The client should construct and send a valid PING packet consisting of PING header and PING payload.

• The PING header includes the following fields:

o “Version” field of a byte length that includes the version number of your ping system. Let the value of this field to be “1” corresponding to Ver

1.0, o “SequenceNo” field of type integer. The value starts at 1 and progresses to 10 for each successive ping message sent by the client,

o “Timestamp” field of type float. The client should set this value to the current time when this packet is constructed,

o “Size” field of type integer that is set to the number of bytes (size) of the payload portion of the ping packet.

• The PING payload includes the following lines o “Host: &lt;hostname&gt;” where &lt;hostname&gt; is the hostname of the client,

• Print the ping request before you send it to the server. The ping header should be printed as:

o ———- Ping Packet Header ———- o Version: &lt;Version field&gt; o Sequence No.: &lt;SequenceNo field&gt; o Time: &lt;Timestep field&gt; o Payload Size: &lt;Size field&gt; o ——— Ping Packet Payload ———— o Host: &lt;hostname&gt;

• When the client receives a reply from the server for the current ping packet the client sent, the client needs to parse the received reply packet and do the following:

o Print the reply packet (header and payload) using the same format described earlier for transmitted ping packets with the exception of the divider lines that should be “———– Received Ping Reply Header ———” and “———- Received Ping Reply Payload ————-”.

o Calculate and print the round trip time (RTT), in seconds. RTT is calculated by calculating the difference between the time the reply packet is received by the client, and the timestamp field in the packet, which was set when the packet was created.

• If the client times out and did not receive a reply for the packet that was just sent, the client needs to print: “————— Ping Reply Timed out —————–”

• After the client is done with the transmitted 10 ping packets, it needs to print a summary of the ping process. In particular the client needs to print the minimum, maximum, and average RTTs at the end of all ping packets. In addition, your client needs to calculate and print the packet loss rate (in percentage).This should be print in the format:

o Summary: &lt;min RTT&gt; :: &lt;max RTT&gt; :: &lt;avg RTT&gt; :: &lt;packet loss rate&gt;

• Once you have this part of the client working, you should test it with your server

PINGServer

• Here, you will develop your own version of a ping server.

• Your server should be named PINGServer.java, PINGServer.py, PINGServer.c, etc.

• The program must accept a single command-line argument: port, which is the port that it will listen on for incoming pings from clients.

o If any of the arguments are incorrect, exit after printing an error message of the form “ERR – arg x”, where x is the argument number. o The only error-checking that needs to be done on the port is to ensure it is a positive integer less than 65536.

o Remember that only ports 10000-11000 are open for use.

• If the program is successful in creating the server socket using the input port number argument, your program should print this out in the form of: “PINGServer’s socket is created using port number &lt;port&gt; with IP address &lt;ip&gt;…”, where &lt;port&gt; is the input argument, and &lt;ip&gt; is the IP address of the server machine.

• If your program as unsuccessful in creating the socket using the input port number argument, it is because this port number is already being taken by another active socket.

o In this case, the program should exit after printing an error message “ERR – cannot create PINGServer socket using port number &lt;port&gt;”, where port is the input argument.

• If the socket is created successfully, the server should sit in an infinite loop listening for incoming UDP packets.

• When a packet arrives, the server simply capitalizes the encapsulated data in the received packet and then sends it back to the client.

• More specifically, in this project, we assume that 30% of the client’s packets will be lost. We will simulate this in the server code in which when a packet arrives to the server, the server will generate a random integer number in the range of [1, 10]. If the randomized integer is less than or equal to 3, the server ignores the received packet (simulating a packet drop). If the randomized integer is greater than or equal to 4, the server resumes normally and handle the received packet as describe earlier.

• For each packet arrives to the server, o You need to print the client’s IP address, port, packet’s sequence number, and whether the packet will be dropped or not in the format IP:port:Seq#:DROPPED in case if the packet will be ignored or

IP:port:Seq#:RECEIVED

Example: 172.18.233.83:63307:56:DROPPED o Print the header and the payload of the received ping packet in the following format:

§ ———-Received Ping Packet Header———-

§ Version: &lt;Version field&gt;

§ Sequence No.: &lt;SequenceNo field&gt;

§ Time: &lt;Timestep field&gt;

§ Payload Size: &lt;Size field&gt;

§ ———Received Ping Packet Payload————  Host: &lt;hostname&gt;

§ User-name: &lt;your last name&gt;, &lt;your first name&gt;

§ —————————————

• Construct a valid response including: 1) the ping response header fields (Version, SequenceNo, Timestamp, Size) that should copy the corresponding values in the received ping packet, and 2) the ping response payload that includes capitalization of each line of the payload of the received ping packet.

• Print the reply packet (header and payload) using the same format described earlier for transmitted ping packets with the exception of the divider lines that should be “———–Ping Reply Header ———-” and “———- Ping Reply Payload ————-”.

• The ping server program should remain running until the user closes it with Ctrl-C.

• Once you have your server working, you could test with your PINGClient.

VM Linux Machines:

• Open “terminal” window either on Windows, Mac, or Unix machine.

• On terminal, type “ssh –l &lt;eID&gt; 172.18.233.74” then your VCU password to authenticate. Note that &lt;eID&gt; is your VCU user login. If success, you will be logged to machine “egr-v-cmsc440-1”

• You can also log to other machines “egr-v-cmsc440-2” and “egr-v-cmsc440-3”. To do so:

• Open a new terminal

• Log first to machine “egr-v-cmsc440-1” as described above using the ssh command.

• Then, once you logged to “egr-v-cmsc440-1”, use “ssh 10.0.0.2” or “ssh

10.0.0.3” to log to “egr-v-cmsc440-2” or “egr-v-cmsc440-3” respectively.

Rules:

• The only programming networking classes allowed are the basic socket classes that we’ve used with the examples. For example, java.net.URL is not allowed and urllib2 in Python is not allowed.

• Your code should run on the VM Linux machines (e.g., 172.18.233.74). Note that only ports 10000-11000 are open for use

• You are not permitted to work with anyone else (even students not in the class) – all of the coding and documentation must be your own.

• Your program must compile (if Java/C++) and run on the VM Linux machines.

• You must write neat code and document it well. You will lose points for sloppy programs that contain little or no comments.

Hints:

• Look back in your notes to recall how UDP client-server network applications are structured.

• If you are using Java, note that readLine() in Java strips off newline characters before returning a String.

• If you are using Java, use the equals() method in Java to compare two Strings.

Testing:

A large part of your program’s grade will be determined by how well it handles a set of inputs. You should test your program rigorously before submitting. Because your programs will be run and tested using a script, you must format your output exactly as I have described, or you will lose points.

Submission Materials:

• Make sure your program compiles and executes on Dept’s VM Linux machines. • Create a “Readme.txt” file for your program that lists how to compile and execute the program. Include your name and your V# as the first line in the Readme.txt.

• You must name your source programs PINGClient.java/PINGServer.java, PINGClient.py/PINGServer.py, or PINGClient.cpp/PINGServer.cpp.

• Submit all files necessary to compile your program.

• Zip all files of your program files in a single zip file and name it prog_assign.zip • Submit through Canvas.

Submitting Assignments using Canvas

– Instructions from the official Canvas help pages

– Step-by-step instructions:

1. Log in to the course Canvas page

2. Click the Assignments link on the left sidebar

3. Click the name of the intended assignment under the

“Programming Assignment” group

4. To submit an assignment, click the Start Assignment button.

5. To upload a file from your computer as your assignment, select the File Upload tab.

7. When you’ve finished adding all files needed for the assignment, click Submit Assignment.

• After you have submitted your work, you will see information on the Sidebar about your submission with a link to your submission to download if necessary

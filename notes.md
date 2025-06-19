
# THIS IS JAVA IMPORTANT QUESTIONS 
* are objects iterable in java or not ?

In Java, an object is iterable if it implements the Iterable interface. For example:

ArrayList , LinkedList , HashSet , TreeSet , HashMap.keySet(), HashMap.values() (not the map itself)

`class Student 
{
    String name;
    int age;
}
`
this is not iterable directly , we need to implements iterable for the plain objects

`class MyContainer implements Iterable<String> {
    private String[] data = {"A", "B", "C"};

    public Iterator<String> iterator() {
        return Arrays.asList(data).iterator();
    }
}
`






# javascript 

* Tell me use of filter and map 


* map -- transform each element in the array

` const numbers = [1,2,3,4,5];
const squared = numbers.map((num)=>num*num) `

------in making todo application we can use map for updation 

* filter --return and array of elements which matches the condition 

`const nums = [1,2,3,4,5];
const even = nums.filter((num)=> num%2==0)`

-------in making todo application we can use filter for delete todos 



# BACKEND
* AUTHENTICATION AND AUTHORIZATION 
-----------------------------------
* Authentication: Verifying who the user is (login/signup).

* Authorization: Verifying what the user can access (admin, user, etc.).

* THERE ARE TWO TYPES OF AUTHENTICATION :-
  -------------------------------------

* Session-Based	----------->> Server stores user session in memory or database. Old method, used with cookies.
* Token-Based (JWT)	----------->> Server issues a signed token (usually JWT), stored in client (localStorage/cookie).






# react 

* we can directly access the local storage until we are at the client side 

* Onclik me hmesha reference de skte hai function ni...but function jaisa dene liye callback Function ka use kr skte hai () => () 




# DBMS / SQL 

* Use on delete cascade 

If we are deleting something from the child table then it will be deleted automatically from the parent table

* Use of on delete set null

 If you are deleted from the parent table then the corresponding child table entry will be set as null

* Can foreign key have null value .
Yes the example is no delete set null


* Can we run select statements without using from ...

Yes , we can ,
SELECT 5+5 ;
SELECT  'hello world';

* When you remove from clause , my SQL treat it as selecting a single row with no columns, it allows you to evaluate expression directly 

* What is happening when we are using a group without any aggregation function

It is allowed but the values for non group columns are undefined or inconsistent


# COMPUTER NETWORK 
--------------------------------------------------------------------------------------------------------------------------------------------
A computer network is a group of two or more computers connected together to share information, data, resources (like files, printers, internet, etc.).

INTERNET -----> The Internet is a huge network that connects millions of computers around the world so they can communicate, share data, and access information.

* why is the computer network so important ?

A computer network is important because it helps computers and devices connect with each other, so they can share information, files, and resources easily and quickly.
A computer network makes everything faster, easier, cheaper, and more connected – whether at home, in school, in offices, or across the world.

* client server architecture -------->
  
Client = The user/device that requests services (like your browser or phone)

 Advantages:
-----------------------
Centralized control of data

Easy to manage and secure

Scalable (can add more clients easily)

Disadvantages:
----------------------
Server failure = everything stops

* What is a Networking Protocol ?

A networking protocol is a set of rules that computers follow to communicate with each other over a network (like the Internet).
Needs good security and hardware
------------------------------------------

HTTP-->	    HyperText Transfer Protocol ----	Transfers web pages over the internet (used in browsers)

HTTPS ---->	    HTTP Secure	   ----                 Same as HTTP but encrypted for security

FTP --->	        File Transfer Protocol	  ----     Used to upload/download files between computers

TCP	 --->       Transmission Control Protocol ---	Ensures reliable and ordered delivery of data

UDP  --->    	User Datagram Protocol	----     Fast but doesn’t check for reliability (used in video calls, gaming)

IP   --->   	Internet Protocol	---------        Sends data between devices using IP addresses

SMTP ---->	    Simple Mail Transfer Protocol -----	Used to send emails

DNS   ---->      Domain name system   ------           convert website name (like google.com) into IP address

* HTTP (HyperText Transfer Protocol)
------------------------------------------
HTTP is the protocol used by web browsers to communicate with web servers.

It allows the transfer of webpages, images, and files from a server to your device

Stateless: Each request is treated independently.

Works on Port 80 by default.

Not secure (data is not encrypted

Know how HTTP GET and POST methods work.

Be able to explain HTTP status codes like:

200 OK

404 Not Found

500 Internal Server Error

* What is SSL/TLS?

🔸 SSL: Secure Sockets Layer

🔸 TLS: Transport Layer Security (newer, more secure version of SSL)

SSL/TLS is a protocol that encrypts data between your browser (client) and a web server, so that no one (like hackers) can read or modify it.

* HTTPS (HyperText Transfer Protocol Secure)
----------------------------------------------------------
Same as HTTP but secure — it uses SSL/TLS encryption to protect data
When you visit a site with https://, it encrypts the communication between your browser and server.
Prevents hackers from reading or tampering with the data

Works on Port 443.
Used for secure login, payments, personal data.


* TCP (Transmission Control Protocol)
---------------------------------------------
TCP ensures reliable communication between devices.
It guarantees that data is delivered, complete, and in the right order.

HOW IT WORKS ---> 
Breaks large data into packets.
Uses a 3-way handshake (SYN, SYN-ACK, ACK) to establish a connection.

If a packet is lost, it resends it.

Key Points:

Reliable, but slower than UDP.

Used in web browsing, email, file transfer.

* What is the TCP 3-Way Handshake?

SYN (Synchronize)
--------------
The client wants to connect.

It sends a SYN packet (a request to start communication) to the server.

SYN-ACK (Synchronize-Acknowledge)
--------------------------
The server receives the SYN.

It replies with a SYN-ACK:

SYN to say “yes, let’s connect”

ACK (Acknowledge)
---------------------
The client receives the SYN-ACK.

It sends an ACK back to the server, confirming the connection is ready.

ACK to acknowledge the client’s request

`Client                               Server

  | ----------- SYN ------------>   |

  | <-------- SYN + ACK ---------  |

  | ----------- ACK ------------>   |

  |        CONNECTION ESTABLISHED  |
`

* UDP (User Datagram Protocol)
------------------------------------------------
A faster alternative to TCP but doesn’t guarantee delivery.

How It Works:
 --------------
Sends data without establishing a connection.

No error checking, no resend, just sends data quickly.

Key Points:
----------
Used in real-time apps like online games, voice calls, video streaming.
"UDP is connectionless, fast, but unreliable. Used where speed matters more than accuracy."

* IP (Internet Protocol)
-----------------------------------------------------------------
IP is used to identify and locate devices on a network using IP addresses.

Sends data packets to the correct destination.

How It Works:
-------------
Every device is assigned a unique IP address (like 192.168.0.1).

Key Points:
--------------
Part of TCP/IP stack.

Two versions: IPv4 (e.g., 192.168.1.1) and IPv6 (longer, more addresses).

IP routes the packets across the network to reach the destination.

Works on Port 53 (DNS), 67/68 (DHCP), etc.


* DNS (Domain Name System)
-----------------------------------------------------------------------
DNS converts domain names like www.google.com into IP addresses

How It Works:
---------
When you type a website name, your device asks a DNS server for its IP address.
The browser then connects to that IP to get the website.

 Key Points:
-------------
Works behind the scenes every time you open a website.

DNS server stores mappings of domain names to IPs.

WHAT HAPPEN WHEN YOU TYPE AN URL ?? 
------> Your browser does not understand domain names like google.com. It needs the IP address (like 142.250.192.4).
------> Your browser uses the IP to connect to the server (e.g., 142.250.192.4).
------> The browser sends an HTTP GET request to the server asking for the web page:
------> The server sends back the HTML, CSS, JS, and image files needed to load the page.
------> Browser reads the code and renders the web page on your screen.

* SMTP (Simple Mail Transfer Protocol)
------------------------------------------------------------
SMTP is used to send emails from your device to the mail server.

How It Works:
-------------
Your email client (like Gmail or Outlook) uses SMTP to send outgoing messages to another server

 Key Points:
-----------------
Works with port 25 or 587.

Can only send emails, not receive them.

* POP3 (Post Office Protocol v3)
-----------------------------------------------

POP3 is used to download emails from the server to your device.
Downloads the email and removes it from the server (unless configured otherwise).

 Key Points:
--------------------------
Good for offline email access.

Works on port 110.

* FTP (File Transfer Protocol)
--------------------------------------------------------------------------

FTP is used to upload or download files between computers over a network.
Connect to an FTP server using username and password, then transfer files.

Key Points:
---------------------------
Used by developers to upload websites or files to web servers.

Works on ports 20 and 21


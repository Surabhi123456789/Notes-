
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
Protocol	Full Form                     	Purpose
HTTP	    HyperText Transfer Protocol 	Transfers web pages over the internet (used in browsers)
HTTPS	    HTTP Secure	                    Same as HTTP but encrypted for security
FTP	        File Transfer Protocol	        Used to upload/download files between computers
TCP	        Transmission Control Protocol	Ensures reliable and ordered delivery of data
UDP      	User Datagram Protocol	        Fast but doesn’t check for reliability (used in video calls, gaming)
IP      	Internet Protocol	            Sends data between devices using IP addresses
SMTP	    Simple Mail Transfer Protocol	Used to send emails
DNS         Domain name system              convert website name (like google.com) into IP address

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

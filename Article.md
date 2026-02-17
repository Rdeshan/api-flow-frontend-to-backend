
                                          this is actaully real internal flow when you start an API call
------------------------------------------------------------------------------------------------------------------------------------------------------
firs we start from the actuall user start process first frontend pass url 
so first step is URL processing :- when there is URL as below 
                 `https://example.com/api/users`   ----> this is the example URL how we pass frontend to backend (API calls)

* https -> protocol
* example.com-> Domain
* /api/users -> path 

     Browser separate those part from the URL , so browser can understand which port this use, this url depend on what connection( http , https )
-------------------------------------------------------------------------------------------------------------------------------------------------------
  then browser check the cahce
  When you type a URL or call an API from your MERN app, the browser does NOT immediately go to the network.
First it checks: “Do I already have this?”
(DNS cache, HTTP cache, and Service Worker cache are all mechanisms used to store data temporarily to improve web performance, reduce latency, and decrease server load)

if cached and valid - it may skip network completely( this didnt establish TCP communication with the server , no network packets pass to the server , everything happen locally or memory )
Response is not cached or expired: Browser must contact the server.TCP 3-way handshake happens → then server sends the data.
---------------------------------------------------------------------------------------------------------------------------------------------------
Assume response is not cached or expired :

DNS REsolution ( finding server IP)
--Before sending anything browser must know what is the IP address of example.com( domain)

Ask DNS server :-example.com -> server IP
first time this ask from DNS server then this save in the browser cache,  )

----------------------------------------------------------------------------------------------------------------------------------------------------
TCP 3way handshake (Establish for connection )

Now the browser try to communicate with server IP, (sendings packets)
Now at this moment both ends know each others IP addresses(client IP and Server IP

     client-----------SYN-------------->server
     server-----------SYN/ACK--------->client
     client-----------ACK-----------> server

Ok now both ends ready to communicate , Once the hanshake is completed with the client and the server communication is open 


     








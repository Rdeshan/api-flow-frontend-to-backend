
                                          this is actaully real internal flow when you start an API call
------------------------------------------------------------------------------------------------------------------------------------------------------
firs we start from the actuall user start process first frontend pass url 
so first step is URL processing :- when there is URL as below 
                 `https://example.com/api/users`   ----> this is the example URL how we pass frontend to backend (API calls)

* https -> protocol
* example.com
* /api/users

     Browser separate those part from the URL , so browser can understand which port this use, this url depend on what connection( http , https )
-------------------------------------------------------------------------------------------------------------------------------------------------------
  then browser check the cahce
  When you type a URL or call an API from your MERN app, the browser does NOT immediately go to the network.
First it checks: “Do I already have this?”
(DNS cache, HTTP cache, and Service Worker cache are all mechanisms used to store data temporarily to improve web performance, reduce latency, and decrease server load)

# WRRC-and-Java :


## The HTTP Request Lifecycle :

* #### Step 1: Local Processing :

* this step depending on the application making the request :


* Your browser extracts the "scheme"/protocol and optional port number, resource path, and query strings .


* #### Step 2: Resolve an IP :

* If the cache lookup fails the browser will fire off DNS request by UDP .

* Whenever the packet hits a piece of networking equipment, the device uses a routing table to determine which other device it is connected to that is most likely situated along the shortest path to the destination.

* Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname.



* #### Step 3: Establish a TCP Connection :

 * when the request was sent over TCP6,
   which is a transport layer protocol like UDP,
   the client must open a TCP connection.


* #### Step 4: Send an HTTP Request :

* after that the client has an IP address and a TCP connection, it can finally send an HTTP request, The request is made up of a "request line", request header, and a body.

* #### Step 5: Tearing Down and Cleaning Up :

* Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal. 

* At this point, your browser begins processing what it has received,and will spin up new requests for that content, restarting this whole process .




## Java HTTP Request example :


* ### HttpUrlConnection :

class  used to perform basic HTTP requests without the use of any additional libraries, but this way has a disadvantage which is using this method are that the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication.
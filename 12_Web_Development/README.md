Homework: Web Development

Questions
Before you work through the questions below, please create a new file and record your answers there. This will be your homework deliverable.
HTTP Requests and Responses
Answer thHomework: Web Developmente following questions about the HTTP request and response process.
1.	What type of architecture does the HTTP request and response process occur in?


         Client-Server Architecture

2.	What are the different parts of an HTTP request?


        Request-Line are these; a) Method b) Request-URL c) HTTP-Version of the request 
        d) Headers and Body 

3.	Which part of an HTTP request is optional?


              The body of the request is optional

4.	What are the three parts of an HTTP response?


             Status Code (2xx, 3xx and so on), Headers and Body

5.	Which number class of status codes represents errors?


          4xx and 5xx classes of status errors, 4xx represents error in client side while 5xx represents error in server side.

6.	What are the two most common request methods that a security professional will encounter?


    GET and POST

7.	Which type of HTTP request method is used for sending data?


          	The POST request

8.	Which part of an HTTP request contains the data being sent to the server?


         The body of the HTTP request contains data sent to the server

9.	In which part of an HTTP response does the browser receive the web code to generate and style a web page?


         The browser receives the web code to generate and style a web page in the body of da response
    Using curl

Answer the following questions about curl:

10.	What are the advantages of using curl over the browser?
    
        •	Spoof user-agent header
         •	View any and all headers on both the response and the request
         •	Set any desired headers
         •	Specify any desired request method

11.	Which curl option is used to change the request method?
      
      
             -X

12.	Which curl option is used to set request headers?
      
      
         -H

13.	Which curl option is used to view the response header?


            -|

14.	Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?
        
        
         Options
        Sessions and Cookies
        Recall that HTTP servers need to be able to recognize clients from one another. They do this through sessions and cookies.

Answer the following questions about sessions and cookies:

15.	Which response header sends a cookie to the client?


          Set-Cookies HTTP/1.1 200 OK Content-Type: text/html Set-Cookie: cart=Bob


16.	Which request header will continue the client’s session?


     Get /cart HTTP/1.1 
    Host: www.example.org
    Cookie: cart=Bob
    ‘Connection: keep-alive’



Example HTTP Requests and Responses
Look through the following example HTTP request and response and answer the following questions:
HTTP Request
POST /login.php HTTP/1.1
Host: example.com
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
Content-Type: application/x-www-form-urlencoded
Content-Length: 34
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Mobile Safari/537.36

username=Barbara&password=password

17.	What is the request method?


        *POST

18.	Which header expresses the client's preference for an encrypted response?


        *Upgrade-Insecure-Requests: 1

19.	Does the request have a user session associated with it?


        *No the session is not reestablished yet

20.	What kind of data is being sent from this request body?


        *Login credentials
          HTTP Response
         HTTP/1.1 200 OK
         Date: Mon, 16 Mar 2020 17:05:43 GMT
         Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT
         Content-Encoding: gzip
         Expires: Fri, 01 May 2020 00:00:00 GMT
        Server: Apache
         Set-Cookie: SessionID=5
         Content-Type: text/html; charset=UTF-8
         Strict-Transport-Security: max-age=31536000; includeSubDomains
         X-Content-Type: NoSniff
          X-Frame-Options: DENY
         X-XSS-Protection: 1; mode=block

[page content]

21.	What is the response status code?


         200

22.	What web server is handling this HTTP response?


         Apache webserver

23.	Does this response have a user session associated to it?


         Yes SessionID=5

24.	What kind of content is likely to be in the [page content] response body?


        Detail of the page configuration

25.	If your class covered security headers, what security request headers have been included?


        Strict-Transport-Security: max-
        Age=31536000; includeSubDomains
       Monoliths and Microservices

Answer the following questions about monoliths and microservices:

26.	What are the individual components of microservices called?


          Services

27.	What is a service that writes to a database and communicates to other services?


        APl’S

28.	What type of underlying technology allows for microservices to become scalable and have redundancy?


           Load Balancer Technology
          Deploying and Testing a Container Set

Answer the following questions about multi-container deployment:

29.	What tool can be used to deploy multiple containers at once?


        Docker

30.	What kind of file format is required for us to deploy a container set?


           .yml YAML format

Databases

31.	Which type of SQL query would we use to see all of the information within a table called customers?


        SELECT column_name FROM customers

32.	Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)


            INSERT INTO table_name (column_1, 2 and 3) (value_1, 2 and 3)

33.	Why would we never run DELETE FROM <table-name>; by itself? 


            It will delete the entire table there is no select statement
________________________________________


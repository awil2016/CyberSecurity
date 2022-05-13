Your Submission:  "Its the End of the Assessment as We Know It, and I Feel Fine"


Guidelines for your Submission:
Provide the following for each phase:


List the steps and commands used to complete the tasks.


List any vulnerabilities discovered.


List any findings associated to a hacker.


Document the mitigation recommendations to protect against the discovered vulnerabilities.


Document the OSI layer where the findings were found.


For example:
Phase 1


Determined the IP ranges to scan were 1.1.1.1 and 2.2.2.2, then ran fping against 1.1.1.1 and 2.2.2.2.


Used the following commands to run fping:

fping 1.1.1.1 





Determined a potential vulnerability that IP 1.1.1.1 is responding.

Since RockStar Corp doesn't want to respond to any requests, this is a vulnerability.



Recommend to restrict allowing ICMP echo requests against IP 1.1.1.1 to prevent successful responses from PING requests.


This occurred on the network layer as Ping uses IP addresses and IPs are used on the Network Layer.
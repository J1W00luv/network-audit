# Home Network Security Audit Using Nmap

## **Aim:**
	To learn about basic commands used to scan networks using Nmap, ports used and do a basic security check.

## **Method:**	
	1. Set up a controlled environment: Run Kali VM & terminal.
	2. Scanning: Find live hosts, scan their ports, assess security.
	3. Analyse the Security: Use information to understand the level of protection that network has.

## **Results:**
	The network scan showed 3 live hosts. One had 4 TCP ports opened (router), the other two had all ports closed. I scanned my router to find more information about its security controls. 
	* SSH (22/TCP) was filtered, meaning it is well protected.
	* DNS (53/TCP) was open and used Cloudflare Public DNS.
	* Web services were available on ports 80 (HTTP) and 443 (HTTPS).
	* Two services were not disclosed. The presence of SSH and restricted fingerprinting suggests firewall rules are well set up from preventing information leaks. 

## **Conclusion:**
	The scan showed how Nmap can be used to do reconnaissance of a network and find potential exposures. The scan provided information about the network's protection and attack surface.

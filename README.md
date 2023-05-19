# InformationGathering
Information Gathering Techiques

# To perform information gathering techniques

# AIM:

To perform information gathering techniques using kali linux 

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:
Open terminal/browser and try execute necessary commands/use url to perform information gathering
### Pen Test Tools Categories:

Following Categories of pen test tools are identified for information gathering:

Footprinting is a part of the reconnaissance process which is used for gathering possible information about a target computer system or network.

http://www.whois.com/whois website to get detailed information about a domain name information including its owner, its registrar, date of registration, expiry, name server, owner's contact information, etc.


## OUTPUT:
![img](https://user-images.githubusercontent.com/118707693/238300689-505c1008-6602-4c30-a18f-a19831193609.png)
### Finding IP address:

ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of saveetha.ac.in.

```
ping saveetha.ac.in
```
![img](s1.png)
## Output:
![img](s2.png)
## Finding Hosting Company

get further detail by using ip2location.com website.
## Output:

![img](s3.png)
## History of the website:
## Output:

https://web.archive.org/
![img](https://user-images.githubusercontent.com/118707693/238300893-192a1d85-246e-45ad-bcd0-0a70e209c601.png)
## Webserver Fingerprinting:
## Netcat:
```
nc 172.17.52.118 80
```
## Output:
![img](s4.png)
## nmap:
```
nmap -p 21 -sV --script=banner ftp.vim.org
```
## Output:
![img](s4.png)
## Whatweb:
```
whatweb infosys.com
```
```
whatweb zoho.com
```
```
whatweb -v -a 3 172.17.52.201
```
## Output:

![Screenshot from 2023-05-15 04-48-16](s5.png)

![Screenshot from 2023-05-15 03-56-55](s6.png)


## httprint:
```
httprint -h 172.17.52.201 -s /usr/share/httprint/signatures.txt -P0 |more
```
## Output:

![Screenshot from 2023-05-15 04-16-42](s7.png)




# Tracing the Location
## TCP Traceroute:
```
sudo traceroute -T www.saveetha.ac.in
```
## Output:


![Screenshot from 2023-05-15 04-51-31](s8.png)



## UDP Traceroute:
```
sudo traceroute -U www.saveetha.ac.in
```
## Output:


![Screenshot from 2023-05-15 04-54-26](s9.png)



## ICMP Traceroute:
```
sudo traceroute  www.saveetha.ac.in
```
## Output:

![Screenshot from 2023-05-15 04-53-50](s10.png)

## RESULT:
The information gathering techniques tools/procedure were  identified successfully

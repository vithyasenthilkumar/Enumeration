# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/672e48cd-bdff-40d3-bea6-e71a504bb773)
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/51cd5a33-0e76-45b8-bd77-3e25cb0c85d9)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/aef55b0e-18e2-4974-aafa-1ecf9eaa3f21)
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/31fe3a2c-b3da-4d35-9af2-c5664f0fe7d0)
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/79c49be8-66ba-498e-bf2f-cae562650f07)
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/29c2b50d-285f-4eb9-8db9-7739afcecc4b)
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
### Output
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/c044539d-c4c3-4667-a2bd-2718d810e7fc)
#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
###OUTPUT
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/7cbad35c-dcb8-4985-9a8f-c2ec98a9483d)
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/19857c23-e614-41a1-990b-cfb41d27ff8a)

##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/accc22c8-4df1-4b92-abb2-7c27e8c98a50)
##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/8497c6d1-32e4-4c1d-a1bf-572b291a396f)
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/0b59891f-04ec-456e-bd3a-6c33336ae743)
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect and issue appropriate commands

![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/91dc7c50-3989-47ab-8677-8552ffd80052)

## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![image](https://github.com/vithyasenthilkumar/Enumeration/assets/127177445/e0c5cb25-2ccd-4e61-a226-0d5054782dfa)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully


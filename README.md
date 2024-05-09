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
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/85979136-dac1-466e-9bfc-d0e414e347a3)


filetype:
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/5687e115-ad88-4d55-81a9-aa8e55c52bbf)

This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/d2deabeb-ae39-4d72-986a-ab2b83ae0b16)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/0ea3dac8-18ad-4576-a7c8-b48b00a02571)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/3340986b-0726-43c7-b079-1ebcdcc20f63)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/47be2ae9-5ed9-461c-95ea-ff12ce9aa9a2)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/80b5bfbf-7902-4ba0-a3fc-9ae6a6b4d6f8)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:







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
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/7733a325-e78f-4f51-a4a3-69f3882792b0)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/b37ea118-c92a-4f3d-b123-64436c609746)

select any username in the first column of the above file and check the same
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/aa129743-a645-4e38-a80b-1202d5953e0c)



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/38bd40b5-3696-4194-9187-b0303c9dcd12)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/jagadeepreddy11/Enumeration/assets/150368525/5198b850-3b73-4fdb-aa6e-808724dd027b)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully


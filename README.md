## Enumeration
## Enumeration Techniques

Explore Google hacking and enumeration

## AIM:
To Compromise windows using Metasploit .

## DESIGN STEPS:
## Step 1:
Install kali linux either in partition or virtual box or in live mode

## Step 2:
Investigate on the various categories of tools as follows:

## Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:
Following Categories of pen test tools are identified: Information Gathering. Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain. Following searches for all the sites that is in the domain yahoo.com
## Output:

![Screenshot 2023-09-19 152926](https://github.com/sakthivel005/Enumeration/assets/120550359/6f329b87-ac04-422d-9b1d-ef1b3595a00e)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files. Following searches for pdf file in the domain yahoo.com

## Output:
![Screenshot 2023-09-19 152947](https://github.com/sakthivel005/Enumeration/assets/120550359/f9515604-01f6-4288-a00f-73d3ce890f3d)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.



## Output:
![Screenshot 2023-09-19 153000](https://github.com/sakthivel005/Enumeration/assets/120550359/69391440-798c-49db-a813-8bf701efca6d)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Ouput:
![Screenshot 2023-09-19 153013](https://github.com/sakthivel005/Enumeration/assets/120550359/ddcee37c-3d45-4ea1-b06f-9e015496bdaf)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.



## Output:
![Screenshot 2023-09-19 153027](https://github.com/sakthivel005/Enumeration/assets/120550359/d4db0014-b4f0-469e-813f-e68e89525239)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.


## Output:
![Screenshot 2023-09-19 153042](https://github.com/sakthivel005/Enumeration/assets/120550359/c05aec34-34c4-4769-b134-6165deabde29)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.


## Output:
![Screenshot 2023-09-19 153100](https://github.com/sakthivel005/Enumeration/assets/120550359/e4a41fad-4a51-4840-83e9-9dc23adc3f57)



#DNS Enumeration

##DNS Recon provides the ability to perform: Check all NS records for zone transfers Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT) Perform common SRV Record Enumeration Top level domain expansion


## OUTPUT:
##dnsenum Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record). Get the namservers (threaded). Get the MX record (threaded). Perform axfr queries on nameservers and get BIND versions(threaded). Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”). Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded). Calculate C class domain network ranges and perform whois queries on them (threaded). Perform reverse lookups on netranges (C class or/and whois netranges) (threaded). Write to domain_ips.txt file ip-blocks. This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

##smtp-user-enum Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

#Telnet for smtp enumeration Telnet allows to connect to remote host based on the port no. For smtp port no is 25 telnet 25 to connect and issue appropriate commands

##Output

nmap –script smtp-enum-users.nse
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

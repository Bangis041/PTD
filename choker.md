## Bismillah. My first medium box on PTD

#### Following the normal process...

## Scanning

```
Nmap scan report for 10.150.150.56
Host is up (0.19s latency).
Not shown: 65530 closed tcp ports (reset)
PORT    STATE SERVICE VERSION
22/tcp  open  ssh     OpenSSH 8.2p1 Ubuntu 4 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 f2:38:1f:67:bf:48:8d:17:a2:5c:66:07:ea:a2:1c:a9 (RSA)
|   256 bb:2d:f9:aa:43:6d:5f:8a:46:ba:83:89:79:f8:f1:65 (ECDSA)
|_  256 47:6a:80:ee:cb:0e:3b:6c:80:db:1b:63:28:dc:91:31 (ED25519)
25/tcp  open  smtp    Postfix smtpd
|_smtp-commands: chocker.localhost, PIPELINING, SIZE 10240000, VRFY, ETRN, STARTTLS, ENHANCEDSTATUSCODES, 8BITMIME, DSN, SMTPUTF8, CHUNKING
80/tcp  open  http    Apache httpd 2.4.41 ((Ubuntu))
|_http-server-header: Apache/2.4.41 (Ubuntu)
|_http-title: Apache2 Ubuntu Default Page: It works
110/tcp open  pop3    Dovecot pop3d
|_pop3-capabilities: SASL(PLAIN LOGIN) RESP-CODES PIPELINING CAPA AUTH-RESP-CODE USER UIDL TOP
143/tcp open  imap    Dovecot imapd (Ubuntu)
|_imap-capabilities: IDLE ID have SASL-IR LOGIN-REFERRALS post-login capabilities LITERAL+ AUTH=PLAIN more AUTH=LOGINA0001 Pre-login IMAP4rev1 OK listed ENABLE
Device type: general purpose
Running: Linux 4.X|5.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5
OS details: Linux 4.15 - 5.19
Network Distance: 2 hops
Service Info: Host:  chocker.localhost; OS: Linux; CPE: cpe:/o:linux:linux_kernel

```

After enumerating hard, http did not give us anything so we move to smtp and the rest to see if we can get anything. We can either do that manually or use msfconsole. Let's see if we can get more users. 

# METASPLOIT ENUM




### Machine name: The Bit

### OS/Rating: Linux/Easy

### Platform: Pwntilldawn(PTD)

### IP: 10.150.150.146

### SCANNING AND ENUMERATION

```# Nmap 7.95 scan initiated Tue Dec  9 00:20:31 2025 as: /usr/lib/nmap/nmap --privileged -p- --min-rate 1000 -sV -A -oN nmap.txt -vvv 10.150.150.146
Nmap scan report for 10.150.150.146
Host is up, received echo-reply ttl 63 (0.19s latency).
Scanned at 2025-12-09 00:20:32 WAT for 306s
Not shown: 65530 closed tcp ports (reset)
PORT     STATE SERVICE  REASON         VERSION
21/tcp   open  ftp?     syn-ack ttl 63
| fingerprint-strings: 
|   GenericLines: 
|     220 ProFTPD Server (ProFTPD) [::ffff:10.150.150.146]
|     Invalid command: try being more creative
|_    Invalid command: try being more creative
22/tcp   open  ssh      syn-ack ttl 63 OpenSSH 8.2p1 Ubuntu 4ubuntu0.1 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 0f:e0:e4:6d:4b:ec:81:f2:e3:53:7f:eb:f0:8b:d1:c6 (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDAFzwivXcWw1UmW7fmriF0BIFr3F0/RYK9F00I8CZ/FZOncHh7h7Wy1iyOBUm1qjG2CEZXjtID1J9WdYUWyCEfC57tM1X6myFfCxXFuOW1YxHRuSNQiopUGl/nvysGZsz5XvR4V/cYgLvVgYsEfXmGV3vWN7T9mnqzDnlhg5sKWVcwMTyaWxlIB+As5WA1HNumjRve2J/fc52LAo15L1hEgwjrjmViC6Db7qUGRr7SUrhTKebj6n8pni1DmW0iFQZTFCM4Hr4vDZyp8fX0Pka2hhiIGgxweR+/us3non5ZgfpMeaFEY63nbmM4g5shSua/jVv2qpf65czP/VFZWlWM4bJLtm+NegXT++l8YXRyzIc6i/U4cHJJ94zN94gTCejVF7/MXrlYu5/nFcYYYwGFAG9Msb7S5zqpmCnZzi0pF6ff20raexlzxqFiMzzgmjfac+krZeQFVMXl1/Q/ejdqoTSeM7UBfP18pXYDoNzsMBvuBJN0YxnZ+N4jiGw5Xc0=
|   256 2c:20:a9:e1:ca:41:7c:a0:b7:81:77:ad:6b:ba:65:8c (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBP3wPGKOZjC06hsa+YIBvylmght2oY9noqzmKwgAbJmlImlmzjsyqwKcyoUgcYG1yfQn5sVMr7e2idYzuF8Md+I=
|   256 70:81:8f:ef:2f:82:cf:52:7c:fb:7e:be:32:93:22:26 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIJ3SSvGEy79IDJlxGlG9Vg2GBGW8ca3yYGlvnYv7nJdU
80/tcp   open  http     syn-ack ttl 63 Apache httpd 2.4.46 ((Unix) OpenSSL/1.1.1i PHP/7.4.14 mod_perl/2.0.11 Perl/v5.32.0)
| http-title: FBC Engineering Reviewer System
|_Requested resource was http://10.150.150.146/reviewer/
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
|_http-server-header: Apache/2.4.46 (Unix) OpenSSL/1.1.1i PHP/7.4.14 mod_perl/2.0.11 Perl/v5.32.0
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
443/tcp  open  ssl/http syn-ack ttl 63 Apache httpd 2.4.46 ((Unix) OpenSSL/1.1.1i PHP/7.4.14 mod_perl/2.0.11 Perl/v5.32.0)
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-favicon: Unknown favicon MD5: 6EB4A43CB64C97F76562AF703893C8FD
| tls-alpn: 
|_  http/1.1
| ssl-cert: Subject: commonName=localhost/organizationName=Apache Friends/stateOrProvinceName=Berlin/countryName=DE/localityName=Berlin
| Issuer: commonName=localhost/organizationName=Apache Friends/stateOrProvinceName=Berlin/countryName=DE/localityName=Berlin
| Public Key type: rsa
| Public Key bits: 1024
| Signature Algorithm: md5WithRSAEncryption
| Not valid before: 2004-10-01T09:10:30
| Not valid after:  2010-09-30T09:10:30
| MD5:   b181:18f6:1a4d:cb51:df5e:189c:40dd:3280
| SHA-1: c4c9:a1dc:528d:41ac:1988:f65d:b62f:9ca9:22fb:e711
| -----BEGIN CERTIFICATE-----
| MIIC5jCCAk+gAwIBAgIBADANBgkqhkiG9w0BAQQFADBcMQswCQYDVQQGEwJERTEP
| MA0GA1UECBMGQmVybGluMQ8wDQYDVQQHEwZCZXJsaW4xFzAVBgNVBAoTDkFwYWNo
| ZSBGcmllbmRzMRIwEAYDVQQDEwlsb2NhbGhvc3QwHhcNMDQxMDAxMDkxMDMwWhcN
| MTAwOTMwMDkxMDMwWjBcMQswCQYDVQQGEwJERTEPMA0GA1UECBMGQmVybGluMQ8w
| DQYDVQQHEwZCZXJsaW4xFzAVBgNVBAoTDkFwYWNoZSBGcmllbmRzMRIwEAYDVQQD
| Ewlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBAMzLZFTC+qN6
| gTZfG9UQgXW3QgIxg7HVWnZyane+YmkWq+s5ZrUgOTPRtAF9I0AknmAcqDKD6p3x
| 8tnwGIWd4cDimf+JpPkVvV26PzkuJhRIgHXvtcCUbipi0kI0LEoVF1iwVZgRbpH9
| KA2AxSHCPvt4bzgxSnjygS2Fybgr8YbJAgMBAAGjgbcwgbQwHQYDVR0OBBYEFBP8
| X524EngQ0fE/DlKqi6VEk8dSMIGEBgNVHSMEfTB7gBQT/F+duBJ4ENHxPw5Sqoul
| RJPHUqFgpF4wXDELMAkGA1UEBhMCREUxDzANBgNVBAgTBkJlcmxpbjEPMA0GA1UE
| BxMGQmVybGluMRcwFQYDVQQKEw5BcGFjaGUgRnJpZW5kczESMBAGA1UEAxMJbG9j
| YWxob3N0ggEAMAwGA1UdEwQFMAMBAf8wDQYJKoZIhvcNAQEEBQADgYEAFaDLTAkk
| p8J2SJ84I7Fp6UVfnpnbkdE2SBLFRKccSYZpoX85J2Z7qmfaQ35p/ZJySLuOQGv/
| IHlXFTt9VWT8meCpubcFl/mI701KBGhAX0DwD5OmkiLk3yGOREhy4Q8ZI+Eg75k7
| WF65KAis5duvvVevPR1CwBk7H9CDe8czwrc=
|_-----END CERTIFICATE-----
|_ssl-date: TLS randomness does not represent time
|_http-server-header: Apache/2.4.46 (Unix) OpenSSL/1.1.1i PHP/7.4.14 mod_perl/2.0.11 Perl/v5.32.0
| http-title: FBC Engineering Reviewer System
|_Requested resource was https://10.150.150.146/reviewer/
3306/tcp open  mysql    syn-ack ttl 63 MariaDB 10.3.24 or later (unauthorized)

```

From the scan seen above, we checked out ftp as it's the first go-to but we did not find anything there as there as we don't have creds and there is no anonymous login. We then proceed to check out other services. Our next line of action is to check out `http`. 

Going to the url http://10.150.150.146, I followed through and landed on a login page 

<img width="1585" height="1004" alt="image" src="https://github.com/user-attachments/assets/528e4f65-b83f-478b-980d-419696cc5c7f" />

First thing I did was check source code to see if there was any information disclosure that would help but nothing so I tried SQLi as per it is a login form.

<img width="941" height="678" alt="image" src="https://github.com/user-attachments/assets/44a7cfd4-e4fe-41aa-8552-4e102603a9a0" />

and boom! 💣💥 we were logged in

<img width="1913" height="565" alt="image" src="https://github.com/user-attachments/assets/92207403-dee1-48a8-b4dd-85657a09c519" />

### THE HUNT FOR SHELL AND FLAGS

I did not have to do much to get the first flag as it was on the web, all I needed to do was play around and check everything that was clickable on the site and I got flag 3

<img width="1920" height="937" alt="image" src="https://github.com/user-attachments/assets/799970b1-0aec-489b-ae7d-72043871ca04" />

After clowning around and not finding anything, I was able to see an image upload function, I decided to test it for file upload vulnerability. Suprisingly it was where I found the first flag. 

<img width="1920" height="886" alt="image" src="https://github.com/user-attachments/assets/756555ca-3a9c-4578-abf7-81f8acdf21c8" />

I just went stright up and uploaded a php file with php extension and a php code in it to get me RCE

<img width="1900" height="946" alt="image" src="https://github.com/user-attachments/assets/bd5f04c3-648a-44d2-8267-bc2d6d842556" />

And now the testing phase...no long story if did not work, you won't see a screenshot below

<img width="1662" height="546" alt="image" src="https://github.com/user-attachments/assets/f9f0d7b2-59a0-4974-bf97-0ab1817bd21e" />

Now to get reverse shell, I used all the commands I know I can use to get reverse shell to my terminal but it's either I have mad skill issue or the thing no just accept am, I sha later uploaded a script to get me shell again. The box was supposed to be named THE UPLOAD 😂.

<img width="983" height="340" alt="image" src="https://github.com/user-attachments/assets/028c8c36-af6a-417f-8c6c-f0d77d5e8280" />

I set up my python server and...

<img width="1709" height="443" alt="image" src="https://github.com/user-attachments/assets/a3fd6d83-96dd-48aa-abff-8ff129d52f9f" />

I wgot my file, and then bashed it after setting up a listener and...you know what happened next, check screenshot below

<img width="1920" height="479" alt="image" src="https://github.com/user-attachments/assets/febc2d22-e74c-47fc-b994-75fa4a26ef5c" />

### Getting root shell

Making the shell stable first, python was no where to be found so I learned how to use `script` to make a shell stable(not in this write-up)




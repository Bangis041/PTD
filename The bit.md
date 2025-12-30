Box name: The bit

Machine/Rating: Linux/Easy

Platform: Pwntilldawn(PTD)

### Nmap Scan

```Nmap scan report for 10.150.150.146
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
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port21-TCP:V=7.95%I=7%D=12/9%Time=69375D92%P=x86_64-pc-linux-gnu%r(Gene
SF:ricLines,92,"220\x20ProFTPD\x20Server\x20\(ProFTPD\)\x20\[::ffff:10\.15
SF:0\.150\.146\]\r\n500\x20Invalid\x20command:\x20try\x20being\x20more\x20
SF:creative\r\n500\x20Invalid\x20command:\x20try\x20being\x20more\x20creat
SF:ive\r\n");
Device type: general purpose
Running: Linux 4.X|5.X
OS CPE: cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:5
OS details: Linux 4.15 - 5.19
TCP/IP fingerprint:
OS:SCAN(V=7.95%E=4%D=12/9%OT=21%CT=1%CU=41019%PV=Y%DS=2%DC=T%G=Y%TM=69375E7
OS:2%P=x86_64-pc-linux-gnu)SEQ(SP=103%GCD=1%ISR=105%TI=Z%CI=Z%II=I%TS=A)OPS
OS:(O1=M508ST11NW7%O2=M508ST11NW7%O3=M508NNT11NW7%O4=M508ST11NW7%O5=M508ST1
OS:1NW7%O6=M508ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6=FE88)ECN
OS:(R=Y%DF=Y%T=40%W=FAF0%O=M508NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F=A
OS:S%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T5(R
OS:=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F
OS:=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R=Y%DF=N%
OS:T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD
OS:=S)
```


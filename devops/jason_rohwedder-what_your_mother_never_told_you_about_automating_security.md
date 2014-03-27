# What your mother never told you about automating security

Jason Rohwedder, Risk I/O, @jasonrohwedder

Where to start? Your app. Continuous integration, continuous deployment.

Agile datacenter. Iterate, iterate, iterate. Production-like development and testing.

Secure hosting? Firehost

Transport security:

* Physical control of network
* Logically isolate network (VLAN / VPC)
* Internal VPN
* SSL all the things
* Audit / SAS70

Network access:

* Host based firewalls (Chef has good recipes)
* Firewall management apps
* AWS - Security groups
* AWS - VPC subnet ACLs

Web Application Firewall

* mod_security cookbook
* incapsula (SaaS)
* darkshield.io (SaaS)

DoS / DDoS protection

* app *bouncer* coming soon
* Incapsula (SaaS)
* Prolexic (SaaS)
* Cloudflare (SaaS)
* Darkshield.io (SaaS)

Bastion host

* Limited services - ssh and VPN for example
* 2-factor authentication

SSH

* Don't use passwords. Keys only.

sudo

* do people still use root? (hah!)

2 factor authentication

* duo-unix cookbook

Servers

* unattended_upgrades
* apt-periodic
* cloudpassage (SaaS)

Software updates

* unattended_upgrades (cookbook)
* apt-periodic (cookbook)
* cloudpassage (SaaS)

OS Hardening

* selinux (cookbook)
* sysctl (cookbook)

IDS

* snort
* ossec
* aide
* cloudpassage (SaaS)
* opsmatic (SaaS) (alpha)

Encrypting data at rest

* encrypted_volume (cookbook) (encrypyted??)
* encryptfs (cookbook)
* zncrypt (cookbook)

Encrypting backups

* encrypted_s3 (cookbook coming soon)
* tarsnap (cookbook)
* network volume with encryption

Logging

* rsyslog (cookbook)
* logstash (cookbook)
* splunk (cookbook)
* graylog2 (cookbook)
* loggly (SaaS)

Testing - test your work as much as you write unit test

* rubygem brakeman
* code climate (SaaS)
* veracode (SaaS and app)

Host vulnerability scanning

* Qualys (SaaS)
* Nessus (app, cookbook)

Webapp vulnerability Scanning

* Whitehat Sentinal (SaaS)
* Qualys (SaaS)

Fixing things

* Risk I/O

War games!

* Demo of security cookbooks reasonable in Chef. Coming this week.

https://github.com/risk-io

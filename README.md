# Cyberdefenders-Boss-of-the-SOC-v1-challenge

##  Incident Response

## scenario 1 from Splunk's site:

Today is Alice's first day at the Wayne Enterprise Security Operations Center. Lucius sits Alice down and gives her first assignment: A memo from Gotham City Police Department (GCPD). Apparently GCPD has found evidence online (http://pastebin.com/Gw6dWjS9) that the website www.imreallynotbatman.com hosted on Wayne Enterprise's IP address space has been compromised. The group has multiple objectives... but a key aspect of their modus operandi is to deface websites in order to embarrass their victim. Lucius has asked Alice to determine if www.imreallynotbatman.com. (the personal blog of Wayne Corporations CEO) was really compromised.


### The investigatation will cover the Cyber Attack Kill Chain from BOTsv1 dataset using Splunk.

### Step 1 - Reconnaissance

1. What is the likely IPv4 address of someone from the Po1s0n1vy group scanning imreallynotbatman.com for web application vulnerabilities?

   Our organization’s website is imreallynotbatman.com.

   Now, we will identify traffic related to the imreallynotbatman.com website.
   by using following query.
   -------------------------------------
   index="botsv1" imreallynotbatman.com
   -------------------------------------

   ![splunk2](https://github.com/user-attachments/assets/a062c715-5d6c-413f-92ee-4602bfee5287)

   There are 78,683 events relating to this website. Currently, not all of them are essential to us.
   We can observe relevant streams as the following:

   ![splunk1](https://github.com/user-attachments/assets/828bf146-0b10-4e6d-aafe-696dcd848645)







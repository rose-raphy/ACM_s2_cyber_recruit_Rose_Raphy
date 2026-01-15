#Challenge-7

Task: Analyze the network traffic, uncover the stolen credentials, log into the system, and retrieve the hidden flag.

Given: login.html,welcome.html,login pcap file, received log, server python file

Analyzis:
1. From the received log from pcap file we know, username: isitadmin, password: iamtheadmin
2. Connect server.py(make sure all the files are in the same place for easier access)
---i used venv to access python3 in linux
---python3 -m venv venv---source venv/bin/activate/---pip install flask---python3 server.py
3. Without closing the linux terminal open the browser and go to link http://127.0.0.1:8080/login
4. Enter username and password
5. Retrieve the flag

Flag: FLAG{analyzing_is_imp}

# SSN Proxy Tutorial

Thank you for your trust in SSN, you will not regret it.

# Suggested specs and details

Operating System: `Ubuntu 20.04`
Ram: `8 Gb`
CPU: `4 core` @ `1 Ghz`
Storage: `3 Gb`

# How To Setup SSN Proxy

# Before we begin, you will want to disable your IPV6 address on your server by running the following 3 commands:

sudo sysctl -w net.ipv6.conf.all.disable_ipv6=1
sudo sysctl -w net.ipv6.conf.default.disable_ipv6=1
sudo sysctl -w net.ipv6.conf.lo.disable_ipv6=1

# SSN Proxy uses JSON to store client data so make sure you read and edit the assets/config.json file.

*   Upload the "PROXY" folder that you received in the "SSNPROXY.zip" onto your server.
*   Replace line 5 in assets/config.json with your server IP

1. `sudo apt install screen -y`

2. `cd PROXY`

3. `chmod 777 *`

4. `./SSNPROXY`

5. CTRL + c

6. `screen -dmS PROXY ./SSNPROXY`

7. `screen -r PROXY`

8. CTRL + a + d

Thats it, you are all setup. Enjoy!

To check out my other services: https://t.me/tcpsyn_feedback
# postgrey-pair-check
A postgrey version that works checking ONLY sender/recipient pair.

By Aobatroz:
This is a modified version of Postgrey 1.34


###
# How to install

[Centos7]
Put the "postgrey" file in /usr/sbin/postgrey. If it's already there, you need to install postgrey 1.34 in your server.


###
# The idea

A triplet checking is not good when we have a sender with lots of differents outcomings IP addresses. Depending on the number of IPs the delivery can never happens if each retry come in a different IP.


###
# The changing

[version 20180215]
Because I manage several e-mails servers at work I needed to act fast, so I changed the way of storing the triplet. Now, the CLIENT_IP is ignored and saved as 0.0.0.0. If you have a better way, please, feel free to change it.

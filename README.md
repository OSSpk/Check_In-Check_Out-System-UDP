# 🙋‍♂️ Check In/Check Out System using UDP
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](#)
[![GitHub Forks](https://img.shields.io/github/forks/harismuneer/Check_In-Check_Out-System-UDP.svg?style=social&label=Fork&maxAge=2592000)](https://www.github.com/harismuneer/Check_In-Check_Out-System-UDP/fork)
[![Build Status](https://semaphoreapp.com/api/v1/projects/d4cca506-99be-44d2-b19e-176f36ec8cf1/128505/badge.svg)](#)
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Check_In-Check_Out-System-UDP.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Check_In-Check_Out-System-UDP/issues)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat&label=Contributions&colorA=red&colorB=black	)](#)


This is a UDP based Check in/Check out System. In this system, the user is able to Check in and Check out from the system by sending a data packet from its host machine. For instance:

User/Client **must** send a message with the following format: 

**YY-AAAA-CI (For check in) (e.g., 12-4159-CI)**

Or

**YY-AAAA-CO (For check out) (e.g., 12-4159-CO)**

where
**(YY-AAAA is your roll number)**

The system/server must get the packet sent by the client and must process the packet accordingly.


## UDP (User Datagram Protocol):
UDP uses a simple **connectionless transmission model** with a minimum of protocol mechanism. With UDP, computer applications can send messages, referred to as datagrams, to other hosts on an Internet Protocol (IP) network without prior communications to set up special transmission channels or data paths. Following are its characteristics:

**1.**	There is no guarantee of delivery, ordering, or duplicate protection.

**2.**	Ideal for network applications where we can tolerate data loss but want to achieve low latency.

## Complete Workflow
The following cases are catered:-

### Check in 
•	Marks the in attendance of the client in a database of the students and returns a welcome message “Welcome Student YY-AAAA”

•	If the user is already checked in it must send the message “You are already here.”

### Check out

•	Marks the out attendance for the client from the student database and then fill the empty place in the database (e.g., if a student initially placed at place 5 has left then all the students above position 5 must come one position down to fill that position). The server must send the message “Good Bye Student YY-AAAA! Have a nice day.”

•	If the user didn’t check in and sent the checkout packet, the server must return the message “You didn’t check in today. Contact System Administrator.”

## Constraints
•	You must print all the members present in the database each time client makes a request to check in or check out.

•	Server must not be restarted once started.

## How to Run
The client. and server.c files are provided. Just compile each file using the following command on Linux terminal or Windows Bash and run it (For client, obviously replace the server.c filename with client.c). Make sure the server is running before running any client.

``` gcc server.c -o server.out ```

----------

## Author
You can get in touch with me on my LinkedIn Profile: [![LinkedIn Link](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=linkedin&longCache=true&style=social&label=Connect
)](https://www.linkedin.com/in/harismuneer)

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/harismuneer)

If you liked the repo then kindly support it by giving it a star ⭐!

## Contributions Welcome
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](#)

If you find any bug in the code or have any improvements in mind then feel free to generate a pull request.

## Issues
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Check_In-Check_Out-System-UDP.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Check_In-Check_Out-System-UDP/issues)

If you face any issue, you can create a new issue in the Issues Tab and I will be glad to help you out.

## License
[![MIT](https://img.shields.io/cocoapods/l/AFNetworking.svg?style=style&label=License&maxAge=2592000)](../master/LICENSE)

Copyright (c) 2018-present, harismuneer                                                        


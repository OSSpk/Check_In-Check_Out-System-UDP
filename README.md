# 🙋‍♂️ Check In/Check Out System using UDP
<a href="https://github.com/harismuneer"><img alt="views" title="Github views" src="https://komarev.com/ghpvc/?username=harismuneer&style=flat-square" width="125"/></a>

[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](#)
[![GitHub Forks](https://img.shields.io/github/forks/harismuneer/Check_In-Check_Out-System-UDP.svg?style=social&label=Fork&maxAge=2592000)](https://www.github.com/harismuneer/Check_In-Check_Out-System-UDP/fork)
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


<hr>



## Author
You can get in touch with me on my LinkedIn Profile: [![LinkedIn Link](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=linkedin&longCache=true&style=social&label=Follow)](https://www.linkedin.com/in/harismuneer)

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/harismuneer)

If you liked the repo then kindly support it by giving it a star ⭐ and share in your circles so more people can benefit from the effort.

## Contributions Welcome
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Check_In-Check_Out-System-UDP.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Check_In-Check_Out-System-UDP/issues)

If you find any bugs, have suggestions, or face issues:

- Open an Issue in the Issues Tab to discuss them.
- Submit a Pull Request to propose fixes or improvements.
- Review Pull Requests from other contributors to help maintain the project's quality and progress.

This project thrives on community collaboration! Members are encouraged to take the initiative, support one another, and actively engage in all aspects of the project. Whether it’s debugging, fixing issues, or brainstorming new ideas, your contributions are what keep this project moving forward.

With modern AI tools like ChatGPT, solving challenges and contributing effectively is easier than ever. Let’s work together to make this project the best it can be! 🚀

## License
[![MIT](https://img.shields.io/cocoapods/l/AFNetworking.svg?style=style&label=License&maxAge=2592000)](../master/LICENSE)

Copyright (c) 2018-present, harismuneer                                                        

<!-- PROFILE_INTRO_START -->

<hr>

<h1> <a href="#"><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" alt="Waving hand" width="28"></a>
Hey there, I'm <a href="https://www.linkedin.com/in/harismuneer/">Haris Muneer</a> 👨🏻‍💻
</h1>


<a href="https://github.com/harismuneer"><img src="https://img.shields.io/github/stars/harismuneer" alt="Total Github Stars"></a>
<a href="https://github.com/harismuneer?tab=followers"><img src="https://img.shields.io/github/followers/harismuneer" alt="Total Github Followers"></a>

<hr>

- <b>🕸️ Founder of Cyfy Labs:</b> At <a href="https://www.cyfylabs.com">Cyfy Labs</a>, we provide advanced social media scraping tools that enable businesses, researchers, and marketers to extract actionable insights from platforms like Facebook, Instagram, and X (formerly Twitter). Our tools are designed for use cases such as lead generation, market research, social listening, and more. Learn more at <a href="https://www.cyfylabs.com">www.cyfylabs.com</a>

- <b>🌟 Open Source Advocate:</b> Passionate about making technology accessible, I’ve developed and open-sourced several software projects for web, mobile, desktop, and AI on my <a href="https://github.com/harismuneer">GitHub profile</a>. These projects have been used by thousands of learners worldwide to enhance their skills and knowledge.

- <b>📫 How to Reach Me:</b> To learn more about my skills and work, visit my <a href="https://www.linkedin.com/in/harismuneer">LinkedIn profile</a>. For collaboration or inquiries, feel free to reach out via <a href="mailto:haris.muneer5@gmail.com">email</a>. For Cyfy Labs related queries, please contact us through our <a href="https://www.cyfylabs.com">company website</a>.

<hr>

<h2 align="left">🤝 Follow my journey</h2>
<p align="left">
  <a href="https://www.linkedin.com/in/harismuneer"><img title="Follow Haris Muneer on LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://github.com/harismuneer"><img title="Follow Haris Muneer on GitHub" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/></a>
  <a href="https://www.youtube.com/@haris_muneer?sub_confirmation=1"><img title="Subscribe on YouTube" src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"/></a> 
   <a href="https://x.com/harismuneer99"><img title="Follow Haris Muneer on Twitter(X)" src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
 <a href="https://www.facebook.com/harism99"><img title="Follow Haris Muneer on Facebook" src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white"/></a>
   <a href="https://www.instagram.com/harismuneer99"><img title="Follow Haris Muneer on Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://www.tiktok.com/@harismuneer99"><img title="Follow Haris Muneer on TikTok" src="https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white"/></a> 
  <a href="mailto:haris.muneer5@gmail.com"><img title="Email" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>



<!-- PROFILE_INTRO_END -->




# MINI-CTF-WRITE-UP
UITM CYBERHEROES CLUB


hiii there....

Greetings! I hope you're all having a splendid day! I kindly request your assistance in unraveling this intriguing puzzle: the enigmatic hacker has concealed something. Our mission is to trace the hacker and uncover their secrets in order to bring this session to a close. Would you be so kind as to lend your expertise and help me out?

.---- ..... ----. .-.-.- -.... ..... .-.-.- .---- ....- ----- .-.-.- ..--- ----- -----

Crack the code and discover the enigmatic hacker! Let's add an extra layer of excitement to this endeavor.

-boredzz-


soo this is how i manage to trace the hacker :)
first when we see the hacker give us a morse code.. from here we can use cyberchef.org to decrypt the code..
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/f380bd4c-aa96-48d7-bf7b-9ed25f0f4bb0)

then i figure out the the output from the morse code is an ip address so i google for it..
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/2152072d-159d-4adb-8d78-0d5fa6e319c4)

so this is the normal login page so i maybee tried sql injection maybe?...or i can scan directory using robots.txt...
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/5def00e1-1c5c-41bf-89d9-27a36f916613)

from this i figure out the /secret directory that may lead me to the hacker so i tried to change robots.txt to secret and boommm...
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/bc85db28-d920-4d21-b89a-1b4e9002ee9a)

so we gain some encyrpt code and im again using cyberchef to decrpyt it by using rot47

before:9EEADi^^:?DE28C2>]4@>^4J36C96C@6D@77:4:2=n:8D9:5l|K#=~sq:}(u=+pll

after:https://instagram.com/cyberheroesofficial?igshid=MzRlODBiNWFlZA==

from here i knew that this is link direct us to cyberheroes official instagram and i open it..
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/5be45dd4-dae1-4d1e-b33e-ca9a089656f2)

and i remember when we open the secret i saw the hacker name which is ./hackboredzz so i try to search from ucc instagram follower...
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/95c59197-12d5-401f-a41c-f71b7de1e9bd)

then we found him and i open his profile and see the first post on 9 june
![image](https://github.com/miroollya/MINI-CTF-WRITE-UP/assets/129681351/46fe5987-1c89-4261-a024-e15e10afb5ef)

then we found out the flag which is UCC{MINI_CTF_PROGRAMME_2023}

enjoy playing? dont forget to follow and share with your friends 
-boredzz-






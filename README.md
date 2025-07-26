# APT-Update-Issue-in-Kali-Linux
Fixing the misconfiguration of source list in Kali Linux
<img width="652" height="184" alt="image" src="https://github.com/user-attachments/assets/a37b2246-dc03-417b-b809-db08ee89ac0d" />

What is wrong here is that your Kali's /etc/apt/sources.list file is either misconfigred or empty. This is the file that tells APT where to look for packages and updates. SInce its empy, it means thet we can neither update nor install anything. Let's fix this...

## Getting Kali Linux's Official Sources

1. Open the file in a text editor. You can use echo, nano, gedit as you prefer: <br>
   
   sudo nano /etc/apt/source.list
   <img width="545" height="84" alt="image" src="https://github.com/user-attachments/assets/65a39342-68de-4f2c-8b6c-8f7145e6fdfd" />

3. Add the sources:<br>

   deb http://http.kali.org/kali kali-rolling main contrib non-free noon-free-firmware
   <img width="931" height="61" alt="image" src="https://github.com/user-attachments/assets/4312ec1b-736b-4b79-8736-eaac67c78a1a" />


4. Save and exit the editor by pressiing:<br>

   CTRL + 0, then Enter to save
   CTRL + X to exit

6. Now run the command to update:<br>

   sudo apt update
   <img width="949" height="138" alt="image" src="https://github.com/user-attachments/assets/b4bf9a33-ed2e-409a-b5a0-bea4c85e1d10" />


Now, your Kali should be able to fetch updates and install packages like it should.

Check the ofiicial documentation here at <a href="https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/">Kali Linux Source List Guide</a>

`#kalilinux` `#APT` `#cybersecurity` `#troubleshooting` `#linufix`

# F.A.Q

# XSS-Finder
- Swiss knife for XSS on any URL,URI,URN,Path,Directory,Parameter,etc
- Any logic is valid logic in this software

# License
- EULA

# Installation
- chmod u+x *
- ./Kali_Installer.sh
- It will become system software

# Run
- Enter in Terminal: ScreamingCobra
- or local directory ./interface.sh

# Screenshot
<div align="center">
    <img src="https://i.ibb.co/4t9Wm0w/xssfinder1.png" width="600px"</img> 
</div>

# Screenshot
<div align="center">
    <img src="https://i.ibb.co/Pg3H3g6/Xssfinder2.png" width="600px"</img> 
</div>

# Screenshot
<div align="center">
    <img src="https://i.ibb.co/sJWbhd8/XSSfinder3.png" width="600px"</img> 
</div>


# DOM Based
<div align="center">
    <img src="https://i.ibb.co/SvSgHPQ/dombased.png" width="600px"</img> 
</div>

# Server Side URL hash (#) feature:
The hash (#) character in a URI denotes the beginning of a URI fragment. According to the RFC 3986, clients are not supposed to send URI fragments to the server, as the client should recognize that they reference a resource secondary to the current, or primary, resource. What does this mean for DOM based XSS! First, the fragment is stored in the DOM as a part of the document.location object, as well as in the document.location.href and document.URL attributes. If a developer parses either of these elements, the fragment will be included. Depending on how the developer parses the URL to extract parameter values, the use of a hash may have no effect on the parser, allowing an attacker to use a hash to inject the payload into the URL, but prevent the payload from being sent to the server where it may be scrutinized. Below is the same example as before, but the exploit is changed by introducing the hash character.

- Example: <script> var x = document.URL.substring(document.URL.indexOf("name=")+5);document.write(name + "!"); </script>
- Exploit: http://example.com?name=Tim#<script>alert(42)</script>
- Result: Hello Tim#<script>alert(42)</script>!

# Payload Information
- Copy paste your payload direct into payload file
- False positive occurs, when file have hidden cr,lf,tb,etc characters
- Be sure your payload file is properly made 


# Appeared
- https://blog.kelvinsecurity.com/2019/09/23/ultimate-swiss-knife-for-finding-xss-in-parameters-uri-url-urn-and-post-based-fuzzing/
- Hacker's Life

# Tweets
- Over, 1000+ tweets

# Official Video
- https://www.youtube.com/watch?v=7zHmizAjQ4o

# Kali Installation
- chmod u+x Kali_Installer.sh
- ./Kali_Installer.sh
- ScreamingCobra
- ScreamingCobra is now system command, call anywhere in system

# Parrot_OS Installation
- chmod u+x Parrot_Os_Installer.sh
- ./Parrot_Os_Installer.sh
- ScreamingCobra
- ScreamingCobra is now system command, call anywhere in system


# Termux Installation
- chmod u+x Termux_Installer.sh
- ./interface.sh

# Compatible
- Android Led TV
- Termux
- Linux
- Windows using cygwin


# URI, URL, Parameters Payloads
- Parameter :
- https://example.com.pk/pages.php?id=

- Fuzzing :
- https://example.com.pk/pages.php?id=id=id=id=

- Exclusives :
- https://example.com.pk/pages.php#
- https://example.com.pk/pages/
- https://example.com.pk/pages.php?id#

# Contact
- mrharoonawna@gmail.com

# Sponsor & Support via BTC
- 3BuUYgEgsRuEra4GwqNVLKnDCTjLEDfptu

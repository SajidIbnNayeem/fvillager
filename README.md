# fvillager
![fvillager](https://github.com/user-attachments/assets/09b7d6d2-87ed-44cf-88b7-dac0e768782f)
<p align="center">
  <img src="https://img.shields.io/badge/Version-1.2.1-green?style=for-the-badge">
  <img src="https://img.shields.io/github/license/SajidIbnNayeem/fvillager?style=for-the-badge">
  <img src="https://img.shields.io/github/stars/SajidIbnNayeem/fvillager?style=for-the-badge">
  <img src="https://img.shields.io/github/issues/SajidIbnNayeem/fvillager?color=red&style=for-the-badge">
  <img src="https://img.shields.io/github/forks/SajidIbnNayeem/fvillager?color=teal&style=for-the-badge">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Author-SajidIbnNayeem-blue?style=flat-square">
  <img src="https://img.shields.io/badge/Open%20Source-Yes-darkgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Maintained%3F-Yes-lightblue?style=flat-square">
  <img src="https://img.shields.io/badge/Written%20In-Bash-darkcyan?style=flat-square">
  <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhtr-tech%2Fzphisher&title=Visitors&edge_flat=false"/></a>
</p>

Concept behind fvillager is simple,
just like we host phishing pages to get credentials why not host a fake page that requests your location like many popular location based websites.
fvillager Hosts a fake website which asks for Location Permission and if the target allows it, we can get :

* Longitude
* Latitude
* Accuracy
* Altitude - Not always available
* Direction - Only available if user is moving
* Speed - Only available if user is moving

Along with Location Information we also get **Device Information** without any permissions :

* Unique ID using Canvas Fingerprinting
* Device Model - Not always available
* Operating System
* Platform
* Number of CPU Cores - Approximate Results
* Amount of RAM - Approximate Results
* Screen Resolution
* GPU information
* Browser Name and Version
* Public IP Address
* Local IP Address
* Local Port


  **Automatic IP Address Reconnaissance** is performed after the above information is received.

**This tool is a Proof of Concept and is for Educational Purposes Only, fvillager shows what data a malicious website can gather about you and your devices and why you should not click on random links and allow critical permissions such as Location etc.**

## How is this Different from IP GeoLocation

* Other tools and services offer IP Geolocation which is NOT accurate at all and does not give location of the target instead it is the approximate location of the ISP.

* fvillager uses HTML API and gets Location Permission and then grabs Longitude and Latitude using GPS Hardware which is present in the device, so fvillager works best with Smartphones, if the GPS Hardware is not present, such as on a Laptop, fvillager fallbacks to IP Geolocation or it will look for Cached Coordinates.  

* Generally if a user accepts location permsission, Accuracy of the information recieved is **accurate to approximately 30 meters**

* Accuracy depends on multiple factors which you may or may not control such as :
  * Device - Won't work on laptops or phones which have broken GPS
  * Browser - Some browsers block javascripts
  * GPS Calibration - If GPS is not calibrated you may get inaccurate results and this is very common
 
## Templates

Available Templates : 

* NearYou
* Google Drive (Suggested by @Akaal_no_one)
* WhatsApp (Suggested by @Dazmed707)
* Telegram
* Zoom (Made by @a7maadf)
* Google reCAPTCHA (Made by @MrEgyptian)

## Tested On :

* Kali Linux
* BlackArch Linux
* Ubuntu
* Fedora
* Kali Nethunter
* Termux
* Parrot OS

## Installation

### Kali Linux / Arch Linux / Ubuntu / Fedora / Parrot OS / Termux

```bash
git clone https://github.com/SajidIbnNayeem/fvillager.git
cd fvillager/
chmod +x install.sh
./install.sh
python3 fvillager.py
```
# Screenshot
![Screenshot From 2024-12-23 19-04-16](https://github.com/user-attachments/assets/c9f55c40-0805-4393-84de-c311107a8ffc)


### Docker

```bash
docker pull SajidIbnNayeem/fvillager
```
# Access Local Services anywhere using Cloudflared (link generate for public)
<li> You must first install cloudflared</li>
  You have to install Cloudflared from their official website
<li> Access local services anywhere using cloudflared</li>
  
  <li> Open a new terminal(new window) and type</li>

```
  cloudflared --url localhost:8080
  ```
![Screenshot From 2024-12-23 19-06-22](https://github.com/user-attachments/assets/ba3efb4f-941b-460f-b3c0-fb7618beb905)

The link will be like this:- https://----------------------------------.trycloudflare.com
![fvillager](https://github.com/user-attachments/assets/cb1cc98d-3cdb-47c0-bd6a-130ed7657c64)

## Screenshot
![screenshot(1)](https://github.com/user-attachments/assets/44ab1b5d-a90e-4ecf-919e-6d3360ebd8d6)

# MadPhisher
![Madphisher](https://github.com/user-attachments/assets/626f68cc-4214-43c6-adbe-c74379865b32)

<p align="center">
  <img src="https://img.shields.io/badge/Version-1.2.4-green?style=for-the-badge">
  <img src="https://img.shields.io/github/license/SajidIbnNayeem/MadPhisher?style=for-the-badge">
  <img src="https://img.shields.io/github/stars/SajidIbnNayeem/MadPhisher?style=for-the-badge">
  <img src="https://img.shields.io/github/issues/SajidIbnNayeem/MadPhisher?color=red&style=for-the-badge">
  <img src="https://img.shields.io/github/forks/SajidIbnNayeem/MadPhisher?color=teal&style=for-the-badge">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Author-SajidIbnNayeem-blue?style=flat-square">
  <img src="https://img.shields.io/badge/Open%20Source-Yes-darkgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Maintained%3F-Yes-lightblue?style=flat-square">
  <img src="https://img.shields.io/badge/Written%20In-Bash-darkcyan?style=flat-square">
  <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhtr-tech%2Fzphisher&title=Visitors&edge_flat=false"/></a>
</p>

<p align="center"><b> A phishing toolkit with 5+ templates.</b></p>

# Disclaimer
<p>Any action and or activities related to <b>MadPhisher</b> is solely your responsibility. The Misuse of toolkit can result in <b>criminal charges</b> brought against the persons in question. <b>The contributors will not held responsible</b> in the event any criminal charges be brought against any individuals misusing this toolkit to break the law.</p>
<b>This toolkit contains materials that can be potentially damaging or dangerous for socialmedia </b>. Referto the laws in your province/country before accessing, using,or in other way utilizing this in a wrong way.
<b>This Tool is made for educational purposes only</b>. Do not attempt to violate the law with anything contained here. <b>If this is your intention, then Get the hell out of her</b>!
it only demonstrates "how phishing works". <b>You shall not misuse the informtion to gain unauthorized access to someones social media</b>.However you may try out this at your own risk.</i>

# Features 
- Latest and updated login pages.
- Beginners friendly

 # Installation
 - Just, Clone this repository -

 ```
  git clone https://github.com/SajidIbnNayeem/MadPhisher.git
 ```

- Now go to cloned directory and run 'Madphisher.sh' - 


```
cd MadPhisher
bash MadPhisher.sh
```
# Screenshots
![Madphisher(1)](https://github.com/user-attachments/assets/6a904c16-5f10-4437-abbd-01384cadad59)
![madphiasher](https://github.com/user-attachments/assets/dfa67585-8223-4d07-8a83-6235df1c2ae4)
![MAdphisher](https://github.com/user-attachments/assets/06d137a5-c164-4ad9-98bb-099f4b6d78c0)

# Access Local Services anywhere using Cloudflared (link generate for public)
<li> You must first install cloudflared</li>
  You have to install Cloudflared from their official website
<li> Access local services anywhere using cloudflared</li>
  
  <li> Open a new terminal(new window) and type</li>
  
  ```
  cloudflared --url localhost:8080
  ```
![screenshot](https://github.com/user-attachments/assets/96f2e07d-36a6-442e-a18f-cbba7b618b13)


- Here you will find another link which you can use - 
  ![Screenshot ](https://github.com/user-attachments/assets/44a5669d-ee00-4847-96eb-455593a2f007)
The link will be like this:- ```https://checking-expires-internet-another.trycloudflare.com```

# Tested On
- Kali Linux -
- Termux -
- Ubuntu -
- Parrot Sec OS -

# Madphisher Termux

 # Installation
 - Just, Clone this repository -

 ```
  git clone https://github.com/SajidIbnNayeem/MadPhisher.git
 ```

- Now go to cloned directory and run 'Madphisher.sh' - 


```
cd MadPhisher
bash MadPhisher.sh
```
![madphisher](https://github.com/user-attachments/assets/144af395-fe7e-4646-92ee-d85c4f9bcc75)


# Termux 
```
pkg update
```
```
pkg upgrade
```
```
git clone https://github.com/SajidIbnNayeem/fvillager.git
```
```
cd fvillager
```
```
chmod +x install.sh
```
```
./install.sh
```
```
python3 fvillager.py
```

# Access Local Services anywhere using Cloudflared (link generate for public)
<li> You must first install Cloudflared-termux</li>
  You have to install Cloudflared-termux from 
  https://github.com/SajidIbnNayeem/Cloudflared-termux.git
<li> Access local services anywhere using cloudflared</li>
  
  <li> Open a new terminal(new session) and type</li>
  
  ```
  cloudflared --url localhost:8080
  ```


### Connect with me:
<div id="badges">
  <a href="https://github.com/SajidIbnNayeem">
    <img src="https://img.shields.io/badge/Github-white?style=for-the-badge&logo=Github&logoColor=black" alt="Github Badge"/>
  </a>
  
   <a href="https://www.instagram.com/sajid_ibn_nayeem?igsh=MXdnNmttb292MnFuaQ==">
    <img src="https://img.shields.io/badge/Instagram-purple?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram Badge"/>
  </a>
   
   <a href="https://twitter.com/Sajid_nayeem_">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>


### Connect with me:
<div id="badges">
  <a href="https://github.com/SajidIbnNayeem">
    <img src="https://img.shields.io/badge/Github-white?style=for-the-badge&logo=Github&logoColor=black" alt="Github Badge"/>
  </a>
  
   <a href="https://www.instagram.com/sajid_ibn_nayeem?igsh=MXdnNmttb292MnFuaQ==">
    <img src="https://img.shields.io/badge/Instagram-purple?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram Badge"/>
  </a>
   
   <a href="https://twitter.com/Sajid_nayeem_">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>






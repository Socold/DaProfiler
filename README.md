![alt text](./files/logo.png)

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![Open Source Love svg3](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/TheRealDalunacrobate/daprofiler)
![](https://visitor-badge.laobi.icu/badge?page_id=TheRealDalunacrobate.daprofiler)

For educational purposes only.

DaProfiler allows you to get emails, social medias, adresses, works and more on your target using web scraping and google dorking techniques, based in France Only. The particularity of this program is its ability to find your targets e-mail adresses.

![alt text](./files/banner.png)
# DaProfiler

DaProfiler allows you to create a profile on your **target** based in France only.
The particularity of this program is its ability to find the e-mail addresses of a target via searches on [Skype](https://www.skype.com/), [Pinterest](https://www.pinterest.com) and tests of combining e-mail addresses followed by a check to know if the email address exists or not (Beware of false negatives, the results displayed do not necessarily relate to the target you are looking for if another person has the same name - first name). DaProfiler is also able to check the words of a an instagram bio to find interesting information such as : **Email addresses**, **Paypal.me profiles**,**Sexual Orientation**,**City**,**School**,**Age**,**Ethnicity**,**Religions**,**Hobbies** and more ...

Official website [www.cnil.me/daprofiler/](https://www.cnil.me/daprofiler/)

## Install

Python 3.8 required
```bash
git clone https://github.com/TheRealDalunacrobate/DaProfiler.git
cd DaProfiler
pip install -r requirements.txt
```
## Use

```bash
profiler.py -n [NAME] -ln [LAST NAME] -l True -O txt_file.txt
(Target Name) (Target Last Name) (Enable Terminal Logging) (Output to txt_file.txt)

=====================================================================

usage: profiler.py [-h] [-n NAME] [-l LOGGING] [-ln LASTNAME] [-O OUTPUT]

  -h, --help            show this help message and exit
  -n NAME, --name NAME  Victim name
  -ln LASTNAME, --lastname LASTNAME
                        Last name of victim
  -u UPDATE, --update UPDATE
                        Update DaProfiler (Optional)
```
### WARNING !
If you are not login to the hub and you search people, your search will be save to the hub. Please register to the hub and use `-pp` to push private your search.


## Demo
![alt text](https://i.ibb.co/XSzG90S/Capture-censored.jpg)

## Api
| Source | Service type | Subscription | Key in code |
| :---: | :---: | :---: | :---: |
| Leakcheck.net | Breach Search | Premium | No | 
| apilayer.net | Phone infos | Free (In code) | Yes |

Add your premium api keys :
+ Go to [modules\api_modules](https://github.com/TheRealDalunacrobate/DaProfiler/tree/main/modules/api_modules) then open your API module (ex Leakcheck), replace "YOUR_KEY" to your key, save and quit your text editor.

# Hub
This branch of daprofiler is supporting the OSINT-HUB integration

> create "./user/key.txt" with your osint-hub key inside see exemple.txt

| Args | Description | Stable |
| :--- | :---------- | :----- |
| -hubR,--hub-register | Permit to register user in the hub | true |
| -hubL,--hub-login | Permet to login to the hub | true |
| -hubU,--hub-username | Set your username | true |
| -hubP,--hub-password | Set your password | true |
| -hubS,--hub-search | Also search on the hub | true |
| -pp,--push-private | Set your search in private | true |
| -pg,--push-group | Set your search in private | true |

## Exemple

### Register to the hub
`python profiler.py --hub-register True --hub-username rabbit --hub-password Aqwzsx1234`

### Search with hub research
`python profiler.py -n amelie -ln delacroix --hub-search True`

> note that a public search use your participation coin :p

## Hub info
Made by: [Alice Snow](https://github.com/Sn0wAlice)<br>
Possible to use a nodejs client to explore: [Here](https://github.com/Sn0wAlice/osint-hub-client)<br>
Website [www.cnil.me](https://www.cnil.me) is the official acces hub website

Admin can delete all your data just if he want ! no need reason !

> educational propose only


# Contact
Mail : _daluna_pro@protonmail.ch_. <br>
Discord : `Dalunacrobate#6166` <br>
Discord server : [Here](https://discord.gg/4h57QSsEYa)


## Contributions
All suggestions are welcome.

## Code parts used under license and authors
+ [Palenath - Instagram Advanced Lookup Function](https://github.com/megadose/toutatis)

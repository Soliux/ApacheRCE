# ApacheRCE

<p align="center">
    <img src="https://media.discordapp.net/attachments/884182203314081812/908371848566300722/download-removebg-preview.png?width=574&height=383" width="320">
</p>


ApacheRCE is a small little python script that will allow you to input the apache version 2.4.49-2.4.50 and then input a list of ip addresses from a text file and mass run the exploit on them, this can be useful if you are running mutiple websites and you want to see if they can all be exploited or not.

DISCLAIMER:
Luckily this will only work if the apache server has CGI enabled on it therefore a large portion of the servers cannot be exploited. As of today `11/11/21` fofa is showing that there are over 145k server running these version combined and I would estimate a good 20-30% of these will have CGI enabled. When creating this script I got a fresh server and installed both apache version on it with CGI enabled and the code works flawlessly

## Installation
Make sure [python](https://www.python.org/) is installed.

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requests.

```bash
pip3 install requests
```

## Usage

```python
python3 exploit.py <version> <ip_file>
```
It is iimportant to note that I am only releasing this script with the intention of system administrators checking their web servers running on the network so that attackers do not use this exploit to get into their network.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

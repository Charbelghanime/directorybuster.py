```
    ___.                   __                
    \_ |__  __ __  _______/  |_  ___________ 
    | __ \|  |  \/  ___/\   __\/ __ \_  __ \\
    | \_\ \  |  /\___ \  |  | \  ___/|  | \/
    |___  /____//____  > |__|  \___  >__|   
        \/           \/            \/          By Charbel Ghanime
```
This tool is designed for security testing purposes to identify accessible directories or paths on a web server by attempting to access them with common directory names. <br>
It performs HTTP GET requests to the specified target website and checks the responses against a user-defined list of valid HTTP status codes. <br>
To start use: <br>
``` git clone https://github.com/Charbelghanime/directorybuster.git ``` <br>
<br>
After successful installation use: <br>
```cd directorybuster ```<br>
To have all the requirements installed use:<br>
```pip install -r requirements.txt``` <br>
To access the help manual: <br>
``` python3 directorybuster.py -h```<br>
or <br>
```python3 directorybuster.py --help ```<br>
To perform a simple scan use:<br>
```python3 directorybuster.py example.com``` <br>
In the example above, directorybuster.py will automatically use the wordlist ```/usr/share/wordlists/dirb/common.txt```<br>
and will show the default status codes: 200, 301, 302, 400, 403, 500, 502. <br>
Other example: <br>
```python3 directorybuster.py example.com -c 200,301,302 -w /usr/share/wordlists/dirb/big.txt```<br>
In this example we are using the tool to show only status codes:200,301,302 and we are using the wordlist:``` /usr/share/wordlists/dirb/big.txt``` <br>
For more options and detailed usage instructions, refer to the help manual: <br>
``` python3 directorybuster.py -h```<br>
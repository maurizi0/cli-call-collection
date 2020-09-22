# Pentesting CLI Call Collection # 

A single grepable file, that contains lots of prototype like CLI calls, of the most common pentesting tool.
Spend less time with man pages ;)

## Exmaple
```bash
grep -i wfuzz clicc.txt    
# wfuzz fuzz a get parameter with; -f out file; --hw hide response with word count; --hh hide response with character count; --hc <code> hide responsecode <code>
wfuzz --hw <word-count> -f <out-file> -w <wordlist> 'https://target.url?param1=FUZZ&param2=42grep -i wfuzz clicc.txt    
```

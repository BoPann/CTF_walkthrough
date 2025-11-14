```
oh so you want to read from keyboard? 
```

### initial thoughts
As always, we start with the classic: `ls -la`.  
Boom—there it is. A mysterious file literally named `-`.
![[Pasted image 20251114114749.png]]

Naturally, your first instinct is to run `cat -` and hope a flag pops out.  
But nope. Plot twist: in Linux, `-` is a special token that means _“read from stdin/stdout.”_

So instead of showing the file, `cat -` basically goes:  
“Oh, you want me to read… your keyboard? Sure buddy.”  
And then it just parrots whatever you type.
![[Pasted image 20251114115005.png]]
### So what do we do?
This challenge is basically trolling you with a cursed filename.  
The workaround? **Escape the filename by giving Linux the actual path**, so it won’t interpret `-` as an option. Extended reading: [[relative vs absolute path]]

Tell Linux, “No no, not stdin — _the file._”  
Relative or absolute path, both work.

### here is the solution command
`cat ./-` (relative path)
`cat /home/bandit1/-` (full path)


And just like that — boom, flag revealed.
![testing](things/Pasted image 20251114113846.png)
![[things/Pasted image 20251114121109.png]]

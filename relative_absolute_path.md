
```
where is it???????
```

### Relative Path

When you type `cat filename` in Linux, you’re basically saying:  
**“Hey Linux, show me this file right here, in _this_ exact directory.”**  
That’s a _relative path_ — you’re referring to the file relative to where you currently are. 

### Absolute Path

But there’s another way: you can give Linux the **entire** address of the file, from the very top of the filesystem all the way down.  
That’s an _absolute path_.

It’s like saying:  
**“No guessing. Go straight from `/` and follow this exact route until you hit the file.”**

For example:

```
cat /home/bandit2/somefile
```

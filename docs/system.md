# System



## Bat & CMD

### Dos Display
**chcp** allows to swtich display mode.
If default display wrong char (like Chinede).

```cmd
chcp 65001 //UTF-8 
chcp 936 //default GBK 
chcp 437 //Eng
```

###  Read File
Read Line in file:

**delims** & **tokens** is like spilt().
Default value **delims = " "**(space), **tokens = 1**
```cmd
for /f %i in (filename.txt) do action //split by space, took the first colume
for /f "delims=" %i in (filename.txt) do action //no split, took all
for /f "tokens=13 delims=、-." %%i in (filename.txt) do ... //split by 、-., took the first and third colume
```



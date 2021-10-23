# **picoCTF**

## **picoGym Practice Challenges**

![picoCTF](https://pbcdn1.podbean.com/imglogo/ep-logo/pbblog8987066/picoCTF_300x300.png "picoCTF")

## **General Skills** 

### *Obedient Cat*

*Steps to follow to solve the challenge*

1. Download the image that gives you the challenge.
2. Open a linux terminal.
3. Go to the directory where the flag file is located using the cd or cd .. command.
4. We use the cat command to visualize what we have said.

```
❯ cat flag
picoCTF{s4n1ty_v3r1f13d_1a94e0f9}
```
5. Copy picoCTF{s4n1ty_v3r1f13d_1a94e0f9} and paste. Finally we upload the answer and complete the challenge successfully.

### Python Wrangling

*Steps to follow to solve the challenge*

1. Execute the wget command to download the ende.py file in the following way
```
❯ wget "https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/ende.py" 
```
2. Execute the wget command to download the pw.txt file in the following way.
```
❯ wget "https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/pw.txt" 
```
3. Execute the wget command to download the flag.txt.en in the following way
```
❯ wget "https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/flag.txt.en" 
```
4. Execute the command python3 ende.py on linux and you will get the following.
```
❯ python3 ende.py
Usage: ende.py (-e/-d) [file]
```
5. Execute the command cat pw.txt on linux and you will get the following.

```
❯ cat pw.txt
192ee2db192ee2db192ee2db192ee2db
```

6. Execute the command python3 ende.py -d flag.txt.en on linux and you will get the following output.

```
❯ python3 ende.py -d flag.txt.en
Please enter the password:
```

7. Copy what we receive when we execute cat pw.txt and paste it where it asks for the password as follows.
```
❯ python3 ende.py -d flag.txt.en
Please enter the password:192ee2db192ee2db192ee2db192ee2db
picoCTF{4p0110_1n_7h3_h0us3_192ee2db}
```
8. We uploaded the following response which is picoCTF{4p0110_1n_7h3_h0us3_192ee2db} and completed the challenge successfully.

### Wave a flag

*Steps to follow to solve the challenge*

1. Execute the wget command to download the warm file in the following way.

```
❯ wget "https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm"
```

2. Let's execute the command ls -l warm to see what permissions the file has and we can see that it does not have execution permissions, only read and write permissions.

```
❯ ls -l warm
-rw-rw-r--
```

3. Let's execute the command chmod +x warm to give the warm file execution permission.

```
❯ chmod +x warm
```

4. We execute the command ls -l warm and we realize that the permissions have changed and we have execution permissions.

```
❯ ls -l warm
-rwxrwxr-x
```

5. We run the command ./warm -h and get the flag which is the following picoCTF{b1scu1ts_4nd_gr4vy_616f7182}. Challenge completed.
```
❯ ./xd -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_616f7182}

```


# learning-the-shell
## Redirecting Standard Output
To redirect standard output to a file instead of the screen, we use the ">" redirection operator followed by the name of the file.
```
Hungs-MacBook-Pro:myLinux hunghoang$ ls > ls-output.txt
```
To view to content of ls-output.txt:
```
Hungs-MacBook-Pro:myLinux hunghoang$ less ls-output.txt 
```
> Linux Device Driver 3rd Edition - O'Reilly.pdf 
> TheLinuxCommandLine.pdf
> ls-output.txt
> playground

Assume we want to append new content to ls-output.txt instead of overwriting it, we'll use the ">>" redirection operator:
````
Hungs-MacBook-Pro:myLinux hunghoang$ ls /Users/hunghoang/Downloads/ >> ls-output.txt 
````

## Redirecting Standard Input
#### The cat command 
This command reads one or more files and copies them to std output, for example:
```
Hungs-MacBook-Pro:myLinux hunghoang$ cat ls-output.txt 
```
will display the content of ls-output.txt 

#### wc - Print line, word and byte counts
The wc (word count) command is used to display the number of lines, words, and bytes
contained in files. For example:
````
Hungs-MacBook-Pro:myLinux hunghoang$ wc ls-output.txt 
      20      28     448 ls-output.txt
````
It means the target file has 20 lines, 28 words and 448 bytes

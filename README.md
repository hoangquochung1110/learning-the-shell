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

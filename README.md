# Ancora-Education-Ucertify-Lab25
# Securing an Apache Web Server

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=8]

## Instructions
In this lab, you will learn to secure your system by hiding information from potential attackers by changing the default location of an Apache folder.

To secure an Apache Web server, here's what you need to do: 

1.From the taskbar, open File Explorer. 

2.In the This PC window, navigate to C: > xampp. 

3.In the xampp window, select htdocs, and press Ctrl+X. 

4.In the Local Disk (C:) window, press Ctrl+V.

Note: Do not copy the subdirectory or else you will lose all the custom permissions that protect the directory.

5.Rename htdocs as webfiles.

6.On the taskbar, in the search box, type Notepad and then right-click and select Run as administrator.

7.In the Notepad window, go to the File tab, click Open, and navigate to C: > xampp > apache > conf. 

8.From the Text Documents (*.txt) dropdown list, select All Files as the file type, then select httpd.conf, and click Open.

9.In the http.conf - Notepad window, perform the following to: 

Scroll down to the following line: 
```bash
DocumentRoot "C:/xampp/htdocs"
```

Modify the line to read as follows:
```bash
DocumentRoot "C:/webfiles"
```

Scroll down to the following line:
```bash
<Directory "C:/xampp/htdocs">
```

Modify the line to read as follows:
```bash
<Directory "C:/webfiles">
```

10.Press Ctrl+S to save the httpd.conf file.

11.Close all the windows.

12.Click Start and from the start menu, navigate to XAMPP > XAMPP Control Panel. 

13.In the XAMPP Control Panel v3.2.2 window, start, stop, and then restart the Apache Web service.

14.Minimize the XAMPP Control Panel v3.2.2 window. 

15.From the desktop, open Google Chrome.

16.In the Google Chrome window, type localhost in the address bar. 

17.You should see your XAMPP splash screen.

18.Close Google Chrome.

## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.

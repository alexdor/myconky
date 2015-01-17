# myconky
Conky scripts

-------------------------------------------------------------------------------------------------------------------

What is a conky?

Conky is a free, light-weight system monitor for X, that displays any information on your desktop. Conky is licensed under the GPL and runs on Linux and BSD. Official website: http://conky.sourceforge.net/

-------------------------------------------------------------------------------------------------------------------

How to install conky on Ubuntu, Mint and Debian?

Open a terminal and type: sudo apt-get install conky conky-all.

Also it is recommended to install curl, lm-sensors and hddtemp (sudo apt-get install curl lm-sensors hddtemp)

-------------------------------------------------------------------------------------------------------------------


How to set a conky?

 1) Create a empty document on your home folder and name it ".conkyrc" (the dot in front of the name makes the file     hidden).
 
  2) Paste the code from a conky script and save the file.
  
  3) Create another empty document on your home folder and name it ".startconky" (we will use it to start conky on       startup).
  
  4) Paste the following code to ".startconky":
  
       #!/bin/bash
       
       sleep 20 &&	
       
       conky -c ~/.conkyrc &
       
  5) Save it and make it executable
  
  6) Go to your startup application and add the ".startconky"
  
  7) Next time you reboot conky should be there. You can start conky by typping "conky -c ~/.conkyrc &" to the         terminal.

You can alternative use the conky manager witch is a gui for using conkys. You can find instruction here: http://www.teejeetech.in/p/conky-manager.html
  

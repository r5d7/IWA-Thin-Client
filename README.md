# IWA-Thin-Client
A collection of bash scripts to watch Infowars on your Raspberry Pi Terminal 

For starters this was ment to watch the Alex Jones show on a raspberry pi 3 at the terminal. As of today everything was working so it's all good. You'll follow the same procedure for the rest of the scripts. 

Download the script and make sure it's executable: 

$ chmod +x ./alex 

Install the script the placing it /usr/local/bin

$ mv ./alex /usr/local/bin

Next edit your /etc/enviornment file and add this:
PATH="/usr/local/bin:/usr/bin:/sbin:/bin:/usr/local/sbin" 

Now you'll want to source this file: 

$ sudo source /etc/enviornment && export PATH
$ source /etc/enviornment && export PATH

You should be good to go all you have to do now is: 

sudo alex

Press Ctrl-C to return to your console. 

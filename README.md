# IWA-Thin-Client

Infowars Army Thin Client

A collection of bash scripts to watch Infowars on your Raspberry Pi Terminal 

I wanted to watch the Alex Jones show on the Raspberry Pi 3 terminal. In order to use the script you'll need omxplayer installed. As of today everything was working so it's all good. You'll follow the same procedure for the rest of the scripts. 

First if you haven't already install omxplayer: 

$ sudo apt-get update && sudo apt-get upgrade && sudo apt-get install omxplayer -y

Download the script and make sure it's executable: 

$ chmod +x ./alex 

Install the script by placing it /usr/local/bin

$ mv ./alex /usr/local/bin

Next edit your /etc/enviornment file and add this:

PATH="/usr/local/bin:/usr/bin:/sbin:/bin:/usr/local/sbin" 

Now you'll want to source this file: 

$ sudo source /etc/enviornment && export PATH
$ source /etc/enviornment && export PATH

You should be good to go all you have to do now is: 

$ sudo alex

Press Ctrl-C to return to your console. 

# Development 

After awhile I'll start working on an install script. The goal would be to have a single script that does all of the above. Then leaves you with the following commands: 

sudo alex |  Watch the Alex Jones Show
sudo knight | Watch Real News with David Knight
sudo owen | Watch the War Room with Owen Shroyer

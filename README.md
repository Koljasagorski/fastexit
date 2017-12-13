# FastExit
Making it easier to run your own Tor Exit Node. This node is defaultly configured to help assist in proactively fighting against abuse from crimeware/malware/spam. It does not eliminate 100% of complaints/abuse.

#Options
Do you want to disable Nginx from logging HTTP requests? (Y/N)
- We highly recommend selecting Y (yes) for this option. This will disable Nginx from logging HTTP requests to the exit node landing page. These logs serve no purpose and could actually harm users who visit the IP via browser if law enforcement decides to seize the server and look through nginx access logs. The goal here is to keep zero logs on the Tor exit server that would be useful in any forensic or legal situation.

#Usage
Log into your server via ssh and download the raw fastexit.sh script and then execute it.<br>
- `wget https://raw.githubusercontent.com/torworld/fastexit/master/fastexit.sh`<br>
- `bash fastexit.sh`

#Notes
Once you run an exit node long enough, you do run the risk of having your personal hosting account information subpoeaned by procecuters/law enforcement if they dont understand that the IP they are investigating is a Tor exit node. If this happens you will have to retain counsel to file a motion to quash the subpoena. If your hosting company is located in the United States; be extra cautious. 

If you have any problems feel free to email us: `security[at]torworld.org`

Visit us at https://TorWorld.org

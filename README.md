# Fixing-VM-Crashing-Hard-Disk
How Hyper V Could Crash your Hard Drive, Plus how to Fixed it.
Real life example...

A friend called me that her laptop was technically crashing. I asked, what did you do before that? "Well, I've ran multiple failed guest machines in my Hyper V in an effort to simulate AD DS and among other things." All these on a 118GB ROM and 8Gb RAM. 

Everytime, a machine failed, remnants are created in the host machine. Until there was no space to run anything. Where did the space she had before starting the VM go? I didn't quite know at first. I've tried every means to figure that out, downloaded tools, checked resources manager, task manager etc. Nothing work. I even deleted every large files on the system, scan it, no fix. 

Hold a sec...what worked? I just remembered from her explanations, it had something to do with virtual machines, so I just hit Windows key +  E, opened the file explorer and typed VHD  for Virtual Hard Drive. There it was. All the big sized failed experiments were there like an uninvited guest that didn't get the memo. I just simply highlighted all and hit delete. Problem fixed.

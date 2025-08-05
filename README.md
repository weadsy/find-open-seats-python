# find-open-seats-python
Check every 10 minutes if a seat opened up in classes of your choosing using API endpoints and python. Includes tutorial for running on Raspberry Pi.

How to run on Raspberry Pi:

1) ssh \<user\>@\<ip\> (connect to the pi, use 'ping raspberrypi.local' to find the ip)

2) python3 --version (make sure python is configured)
   	- (if not configured)
	- sudo apt update
	- sudo apt install python3
	- sudo apt install python3-pip

4) git clone https://github.com/weadsy/find-open-seats-python.git (clone the repo)

5) cd find-open-seats-python (enter the repo)

6) python3 -m venv venv (create virtual environment)

7) source venv/bin/activate (activate virtual environment)

8) pip install requests (install request library)

9) tmux (optional, if you want the script to keep running after you disconnect from ssh. Can also use 'screen')

10) python check_classes.py (run the script)

tmux attach -t 0 (reattach to the session, use 'tmux ls' to see running sessions).

tmux kill-session -t 0 (end the session)

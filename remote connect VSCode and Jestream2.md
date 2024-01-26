# Connecting with VSCode 
- Download and install VSCode: https://code.visualstudio.com.
- In the extensions tab in VSCode, install the **Jupyter** and **Remote--SSH** extensions locally.
- Click the icon to connect to remote host in the bottom-left corner of the VSCode window, then select "Connect to Host" near the search bar.
- Choose "Add New SSH Host", then enter the command ssh exouser@remote-ip-address in the resulting bar. When prompted for a password, enter it (both remote-ip-address and the corresponding password will be provided to teams the day of the event).
- In the extensions tab again, install the **Jupyter** and **Python** extensions on the remote machine.
 
# Connecting with Terminal
- (Windows only) Download and install mobaxterm: https://mobaxterm.mobatek.net
- In a terminal window, run the command ssh exouser@remote-ip-address. When prompted for a password, enter it (both remote-ip-address and the corresponding password will be provided to teams the day of the event).
- Run the commands tmux and jupyter notebook on the remote machine.
- In a new local terminal window, run the command ssh -L localhost:8888:localhost:8888 exouser@remote-ip-address
- In a browser window, enter "localhost:8888".

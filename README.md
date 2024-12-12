Run Nexus Prover Beta
Info
You need to have min 4 RAM in your system (VPS)
Recommended : 6 GB RAM
You can buy VPS from PQ Hosting using cryptocurrency
This script is compatible with Ubuntu on local system as well as on VPS

If you run on VPS, u don't need to do anything after running the installation commands
If you run on Local system (Ubuntu), u just need to open the terminal after turning on your system to start this prover, it will start running automatically again, if it is not running then use this command to run

1st Command `sudo systemctl start nexus.service`

Installation

2nd coomand `curl -sSL https://raw.githubusercontent.com/mobinkhan/nexus-prover/main/nexus.sh | bash`

Or this command to run this script

3rd command `wget -qO - https://raw.githubusercontent.com/mobinkhan/nexus-prover/main/nexus.sh | bash`

You can check prover status using this command

4rd coomand `systemctl status nexus.service`

To check logs, use the below command

5th Command `journalctl -u nexus.service -f -n 50`

4 
Now open terminal and use the below command
sed -i 's/.*/YOUR_PROVER_ID/' .nexus/prover-id
Make sure to replace YOUR_PROVER_ID with the value u copied earlier (Example : sed -i 's/.*/P2Fn8XlXjuWr8yeoJvE6bi2iP1I3/' .nexus/prover-id)
Now restart the nexus.service using below command

`  sudo systemctl restart nexus.service`

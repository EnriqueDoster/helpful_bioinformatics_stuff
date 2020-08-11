# TAMU server use SOP

# Table of contents
* Computing servers
* Example AMR++ run


# Computing servers

# Example AMR++ run
1. Sign-in to a server, ada.
  * Log on to VPN (Anyconnect) if you are not on TAMU’s network, connect.tamu.edu
2. Enter username and password
```
ssh enriquedoster@ada.tamu.edu
```
3. Navigate the server directories
/scratch/user/$USER

4. Prepare directory for running AMR++
module load Singularity/2.5.2-GCC-6.4.0-2.28

# linux-iam-lab
Goal: Set up least-privilege access for a  user on Ubuntu in Azure.
What I did: Created user, added to  group, removed from , tested permissions.
Test: Ran  as  and got .
Why it matters: Shows I understand IAM principles - least privilege, testing, verification.
Next step: Automate this with bash/Bicep.

**#Commands used**
sudo useradd -m devops
sudo groupadd engineers
sudo usermod -aG engineers devops
sudo deluser devops sudo
sudo mkdir /opt/appdata
sudo chgrp engineers /opt/appdata
sudo chmod 770 /opt/appdata

<img width="947" height="761" alt="Screenshot 2026-05-14 165128" src="https://github.com/user-attachments/assets/ab348082-5e01-4d99-a993-129739cff052" />
<img width="315" height="312" alt="Screenshot 2026-05-14 165115" src="https://github.com/user-attachments/assets/fe174049-c118-4e18-81f7-7665c5b681af" />
<img width="898" height="602" alt="Screenshot 2026-05-14 164038" src="https://github.com/user-attachments/assets/d4e427d6-8a1d-46d8-8f94-d6541fac2787" />


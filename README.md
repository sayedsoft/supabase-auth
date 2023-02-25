# Supabase Docker

Create file run-quick.sh

```sh
touch run-quick.sh && chmod +x ./run-quick.sh
```

paste this code by nano editor

```sh
echo "Int before Setup"
echo " by AHMAD YAMAN SAYED"
sudo apt -y upgrade
sudo apt update
sudo apt -y install curl gnupg ca-certificates lsb-release apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
echo "Setuping docker"
sudo apt -y install docker-ce docker-compose
git clone https://github.com/sayedsoft/supabase-auth.git
cd ./supabase-auth && docker-compose up -d
```

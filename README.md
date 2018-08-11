# ssh-login
#tao file ssh publish key
mkdir ~/.ssh; touch ~/.ssh/authorized_keys; chmod 700 ~/.ssh
#mo file dan publiush key
nano ~/.ssh/authorized_keys
#phan quyen
chmod 600 ~/.ssh/authorized_keys
# tuong tu cho cac user khac
/home/user/.ssh/authorized_keys
# khong cho login bang password
sudo nano /etc/ssh/sshd_config
# yes thang no
PasswordAuthentication no
# tim va chuyen nhu mau
PubkeyAuthentication yes
ChallengeResponseAuthentication no
#reset lai ssh
sudo systemctl restart ssh

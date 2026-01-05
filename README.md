ssh -i Practice_key.pem ec2-user@13.211.254.140
EC2側
cd ~/app
git pull
source .venv/bin/activate
python -m pip install -r requirements.txt   # requirements を変えた時だけ
sudo systemctl restart streamlit

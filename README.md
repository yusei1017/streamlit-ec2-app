ssh -i Practice_key.pem ec2-user@13.211.254.140
ローカル
git add.
git commit -m "Update title to v3"
git push

EC2側
cd ~/app
git pull
source .venv/bin/activate
python -m pip install -r requirements.txt   # requirements を変えた時だけ
sudo systemctl restart streamlit

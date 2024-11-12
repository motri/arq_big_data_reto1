1. Set AWS credentials at ~/.aws/credentials
2. Download SSH private key at ~/.ssh/vockey.pem
3. Set the proper permissions for the key: `chmod og-rwx ~/.ssh/vockey.pem`
4. Create a Python virtual environment: python3 -m venv ~/ansible
5. Activate the virtual environment: source ~/ansible/bin/activate
6. Clone the repository: git clone https://github.com/memaldi/atbd-24-25-entrega-1
7. Access to `atbd-24-25-entrega-1`: cd atbd-24-25-entrega-1
8. Install requirements: `pip install -r requirements.txt`
9. Install nginx log generator: `ansible-playbook -i inventory.aws_ec2.yml --key-file=~/.ssh/vockey.pem --user ec2-user install-nginx.yml`
7. Nginx logs can be accessed at /home/ec2-user/log/nginx.log 

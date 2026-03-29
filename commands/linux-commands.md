# Update

sudo yum update -y

# Install Apache

sudo yum install httpd -y

sudo systemctl start httpd
sudo systemctl enable httpd

# Install PHP & MySQL

sudo yum install php php-mysqlnd -y
sudo dnf install mariadb105-server -y

# Install Git

sudo yum install git -y

# Clone Application

git clone https://github.com/onlinebookstore/

# Restart Apache

sudo systemctl restart httpd

# Deploy-Website-on-EC2-TechMax
Deploy Website on EC2

Clone this repository 

<a href="https://github.com/azeezsalu/techmax"> https://github.com/azeezsalu/techmax


```html
https://github.com/azeezsalu/techmax.git
```

## Create a EC2 Instance

<img src="https://github.com/vaibhavkapase1302/Deploy-Website-on-EC2-TechMax/blob/main/EC2%20Instance%20Launch.png"  alt="EC@ Instance Launch">


## Connect EC2 Instance to SSH

#### Ec2 connect through CLI SSH
* Open Windows CLI 
* wite in terminal ```ssh -i "key-pair name" ec2-user@ip-address```

Type these commands in cmd

```
sudo su
```

```
yum update -y
```

```
yum install -y httpd
```

```
cd /var/www/html
```

```
wget https://github.com/azeezsalu/techmax/archive/refs/heads/main.zip
```

```
unzip main.zip
```

```
cp -r techmax-main/* /var/www/html/
```

```
rm -rf techmax-main main.zip
```

```
systemctl enable httpd
```

```
systemctl start httpd
```

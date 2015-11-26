# AWS SES NodeJS Example

Follow the instructions below on an EC2 Ubuntu instance. This tutorial will help you setup the AWS SDK using NodeJS. There are a few endpoints to send email with attachments, create a verified sender, delete a verified sender, and list all of your verified senders. If you have any questions please contact me!

```
sudo su
apt-get update
apt-get upgrade -y
apt-get dist-upgrade -y
apt-get autoremove -y
apt-get install nodejs npm git -y
ln -s /usr/bin/nodejs /usr/bin/node
git clone https://github.com/andrewpuch/aws-ses-node-js-examples.git
cd aws-ses-node-js-examples
npm install
cp config-sample.json config.json
```

***NOTE: Here you will want to edit config.json with your AWS keys and in app.js you will want to edit the email address with your own email address. For this tutorial we will just send email to ourselves.***

```
node app.js
```

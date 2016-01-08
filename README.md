# notify
Start a process and notify via email or SMS when it completes

## Install
```
echo "email=you@email.com" >> ~/.notify
echo "sms=tendigitphonenumber@provideremail.com" >> ~/.notify
export PATH=~/notify:$PATH
```

## Example Usage
Start some_long_running_process and notify when finished
```
notify sh some_long_running_process.sh
```
Send the data listing when new data arrives at a remote server
```
watch -n 60 -g "ssh root@ftp 'ls /var/www'" ; notify ssh root@ftp 'ls /var/www'
```

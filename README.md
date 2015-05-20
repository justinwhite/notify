# notify
Notify me when a process completes

## Install
```
echo "email=you@email.com" >> ~/.notify
export PATH=~/notify:$PATH
```

## Goals
- pipe to notify to notify when done, regardless of error
- find a running process and notify when done

## Example Usage
```
notify bin/some_long_running_process.sh
```

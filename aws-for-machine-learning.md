
# Useful AMIs

- [Deep Learning AMI Ubuntu Version](https://aws.amazon.com/marketplace/pp/B06VSPXKDX): `ami-c5afaaa3`

# Using awscli

## Start an instance

```
$ aws ec2 run-instances --image-id ami-c5afaaa3 --security-group-ids sg-11436668 --count 1 --instance-type p2.xlarge --key-name lskey3 --subnet-id subnet-7a85421d 
```

## List running instances ids

```
$ aws ec2 describe-instances --filters "Name=instance-state-code,Values=16" | jq '.Reservations[].Instances[].InstanceId' 
```

## Get public IP addresses of running instances

```
$ aws ec2 describe-instances --filters "Name=instance-state-code,Values=16" | jq '.Reservations[].Instances[].PublicIpAddress'
```

## Stop an instance

```
$ aws ec2 stop-instances --instance-ids $INSTANCE_ID
```

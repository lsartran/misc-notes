
# Useful AMIs

- [Deep Learning AMI Ubuntu Version](https://aws.amazon.com/marketplace/pp/B06VSPXKDX): `ami-c5afaaa3`

# Using awscli

## Start an instance

```
$ aws ec2 run-instances --image-id ami-c5afaaa3 --count 1 --instance-type p2.xlarge --key-name lskey3 --subnet-id subnet-7a85421d
```

## List instances ids

```
$ aws ec2 describe-instances | jq '.Reservations[].Instances[].InstanceId' 
```

## Stop an instance

```
$ aws ec2 stop-instances --instance-ids $INSTANCE_ID
```

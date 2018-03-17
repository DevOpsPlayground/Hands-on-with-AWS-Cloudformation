# Environment Setup

1. IAM - Create User for Console Access with least privilege.
1. IAM - Create a Service Role for CloudFormation for Labs
1. Check AWS playground has enough limits or request more
1. Test labs
1. Test labs with a group of people
1. Wifi password
1. EitherPad


## IAM Setup

1. User Account `pg19meetup`
  - No Permissions
  1. Create group `meetups`
1. Service Role `pg19meetupLabsRole`

## EC2 Setup

1. Generate EC2 Keypair `pg19meetup`

## AWS CLI Setup

Can can follow the labs using the AWS CLI for this you will need to install the CLI on to your system (see ref[1]).

```
pip install awscli --upgrade --user
```

## References
1. AWS docs - [Install the AWS Command Line Interface on Linux](https://docs.aws.amazon.com/cli/latest/userguide/awscli-install-linux.html)

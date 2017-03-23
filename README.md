# get-dns-of-elb

Get the dns of an ELB append it in the elb dictionary and return it 

## Role Variables

* `elb`      : Dictionary containing the information of the Elastic Load Balancer
  * `name`   : The name of the ELB
  * `region` : The AWS region to use. If not specified then the value of the AWS_REGION or EC2_REGION environment variable, if any, is used. See http://docs.aws.amazon.com/general/latest/gr/rande.html#ec2_region [Default: (null)]

## Example playbook

```yaml

- hosts: localhost
  connection: local
  gather_facts: no
  roles:
    - get-dns-of-elb
```

## License

GPLv2

## Author Information
jamatute (jamatute@paradigma.com)

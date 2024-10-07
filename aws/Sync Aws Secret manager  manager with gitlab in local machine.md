to use Aws secret manager in local machine or in gitlab pipeline by using Aws cli integration in machine and gitlab runner
after installing aws cli into local and gitlab runner you have to configure aws cli with access key id and acceess key decret key and region of your aws

```bash
- echo "Setting up AWS CLI"
    - aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID_PROD
    - aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY_PROD
    - aws configure set region $AWS_DEFAULT_REGION_PROD
```


after installing the aws and configuration you can access secret manager you can get collective string of secrets or can get by specific id or name eg.


```bash
aws secretsmanager get-secret-value --secret-id testvariableforawssecreate --query 'SecretString' --output text

```

![[Screenshot from 2024-10-07 15-17-09.png]]
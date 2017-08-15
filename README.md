# Notes


## Test API

```
apig-test \
--username='email@email.com' \
--password='Password' \
--user-pool-id='ap-northeast-1_xxxxxxxxx' \
--app-client-id='xxxxxxxxxxxxxxxxxxxxxxxx' \
--cognito-region='ap-northeast-1' \
--identity-pool-id='ap-northeast-1:xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx' \
--invoke-url='https://xxxxxxxxxx.execute-api.ap-southeast-1.amazonaws.com/prod' \
--api-gateway-region='ap-southeast-1' \
--path-template='/notes' \
--method='POST' \
--body='{"content":"hello world","attachment":"hello.jpg"}'
```

## Verify User Signed Up

```
aws cognito-idp admin-confirm-sign-up \
   --region ap-northeast-1 \
   --user-pool-id  ap-northeast-1_xxxxxxxxx\
   --username email@email.com
```

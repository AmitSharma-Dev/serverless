## Deploy
1. npm i -g serverless
2. serverless config credentials --provider aws --key {{iamKey}} --secret {{iamSecret}}
3. serverless deploy

## Test
2. create user : 
    POST ${BASE_DOMAIN}/users HTTP/1.1
    content-type: application/json

    {
        "userId": "amit1",
        "name": "amit sharma"
    }

3. retrieve the user : 
    GET ${BASE_DOMAIN}/amit1 HTTP/1.1
    content-type: application/json
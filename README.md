## Local Development
start local server : sls offline start
installing local dynamoDB : sls dynamodb install

## Deploy
1. npm i -g serverless
2. sls config credentials --provider aws --key {{iamKey}} --secret {{iamSecret}}
3. sls deploy

## Test
create user : 
    POST ${BASE_DOMAIN}/users HTTP/1.1
    content-type: application/json

    {
        "userId": "amit1",
        "name": "amit sharma"
    }

retrieve the user : 
    GET ${BASE_DOMAIN}/amit1 HTTP/1.1
    content-type: application/json
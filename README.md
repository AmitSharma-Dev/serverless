# AngularS3

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.1.4.

## Serverless steps followed
1. ng new {{projectName}}
2. npm i -g serverless
3. serverless config credentials --provider aws --key {{iamKey}} --secret {{iamSecret}}
4. ng add @ng-toolkit/serverless --provider aws
5. npm run build:serverless:deploy

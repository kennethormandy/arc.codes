# Lambda functions simplified

<div style=background:lightblue;padding:10px;border-radius:7px;>`.arc` is a plaintext manifest for defining next generation cloud infrastructure</div>

- **Create cloud infra in minutes** from an `.arc` manifest and version control your architecture
- **Deploy in seconds** with first class support for `staging` and `production`
- **Work locally** while completely offline with a speedy in-memory database
- **Primitives not Frameworks**; define app architecture agnostic of vendor arcana

Leverage powerful Amazon Web Services cloud primitives without frustrating configuration: 

- [Lambda](https://aws.amazon.com/lambda/) for compute 
- [API Gateway](https://aws.amazon.com/api-gateway/) for HTTP route handlers
- [Route53](https://aws.amazon.com/route53) for DNS
- [CloudFront](https://aws.amazon.com/cloudfront/) for CDN
- [S3](https://aws.amazon.com/s3/) for static assets
- [Simple Notification Service](https://aws.amazon.com/sns/) for event pub/sub functions
- [CloudWatch Events](https://docs.aws.amazon.com/lambda/latest/dg/with-scheduled-events.html) for scheduling functions
- [DynamoDB](https://aws.amazon.com/dynamodb/) for data persistence, querying and trigger functions

Everything starts with an `.arc` file:

```arc
# this is an .arc file
@app
testapp

@html
get /
get /hellos
post /hello
```

`npm run create` to generates lambda function code locally:

```bash
/
|- src
|  '- html
|     |- get-index/
|     |- get-hellos/
|     '- post-hello/
|- .arc
'- package.json
```

And `npm run deploy` ships your code to the cloud in seconds. <span class=cloud>&#x1f329;</span>

## Next steps

- [Follow the quickstart](/quickstart)
- [Read the reference](/reference)

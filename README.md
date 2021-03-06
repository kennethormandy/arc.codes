# <kbd>:cloud_with_lightning: [`arc.codes`](https://arc.codes)</kbd>

> https://arc.codes

[ ![Codeship Status for arc-repos/arc.codes](https://app.codeship.com/projects/69a79dc0-4fd3-0135-6f18-062897f7455f/status?branch=master)](https://app.codeship.com/projects/234163)

## Setup

0. To deploy, first set up a `[jsf]` profile in `~/.aws/credentials` with stubbed `aws_access_key_id`, `aws_secret_access_key`, and `region` env vars.
1. Ensure that `arc-docs` is a sibling of this repo.
2. Initialize the repos by running `npm i && npm run init`.
3. Link to your local copy of `arc-docs` by running `npm run link ../arc-docs/`.

## Test

```
npm it
```

## Preview

```
npm start
```

## Deploy

Anything that hits master green gets deployed automatically. You can deploy whatever you have locally by running:

```
ARC_DEPLOY=production npm run deploy
```

### TODO

- get dns setup for staging

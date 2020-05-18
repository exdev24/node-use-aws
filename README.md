# CasperJS AWS Lambda Template

A [CasperJS](http://casperjs.org/) node.js app for [Amazon Lambda](http://aws.amazon.com/lambda/).
Based on [node-lambda-template](https://github.com/rebelmail/node-lambda-template) using [node-lambda](https://github.com/rebelmail/node-lambda).
The app includes a [PhantomJS](http://phantomjs.org/) binary (i.e., in the `/bin/` directory named: `phantomjs`) compiled for AWS Linux (https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-1.9.8-linux-x86_64.tar.bz2).

**Note:** If you want to use different PhantomJS binary in your project, then you will be need to download a latest binary from [here](https://bitbucket.org/ariya/phantomjs/downloads/) and replace it with `/bin/phantomjs` (i.e., Make sure you keep the name as is for now).

**There are the 3 available commands:**

- setup: `$ npm run setup`
- start: `$ npm run start`
- deploy: `$ npm run deploy`


To run the function locally execute the following command:
```shell
$ ./node_modules/.bin/node-lambda run
# OR
$ npm run start # yarn start
```

Run the following command to deploy the app to Amazon Lambda:
```shell
$ ./node_modules/.bin/node-lambda deploy
# OR
$ npm run deploy # yarn deploy
```

For running tests:
```shell
$ npm run test # yarn test
```

For more about commands visit `node_lambda` [repository here](https://github.com/motdotla/node-lambda)
> **Note:** npm version 2.x or newer required to pass arguments to the scripts using `-- args`
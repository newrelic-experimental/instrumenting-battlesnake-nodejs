# Instrummenting your BattleSnake with New Relic using NodeJS

[![New Relic Experimental header](https://github.com/newrelic/opensource-website/raw/master/src/images/categories/Experimental.png)](https://opensource.newrelic.com/oss-category/#new-relic-experimental)


![GitHub forks](https://img.shields.io/github/forks/newrelic-experimental/instrumenting-battlesnake-nodejs?style=social)
![GitHub stars](https://img.shields.io/github/stars/newrelic-experimental/instrumenting-battlesnake-nodejs?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/newrelic-experimental/instrumenting-battlesnake-nodejs?style=social)

![GitHub last commit](https://img.shields.io/github/last-commit/newrelic-experimental/instrumenting-battlesnake-nodejs)

![GitHub issues](https://img.shields.io/github/issues/newrelic-experimental/instrumenting-battlesnake-nodejs)
![GitHub issues closed](https://img.shields.io/github/issues-closed/newrelic-experimental/instrumenting-battlesnake-nodejs)
![GitHub pull requests](https://img.shields.io/github/issues-pr/newrelic-experimental/instrumenting-battlesnake-nodejs)
![GitHub pull requests closed](https://img.shields.io/github/issues-pr-closed/newrelic-experimental/instrumenting-battlesnake-nodejs)

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](CODE_OF_CONDUCT.md)
[![Apache licensed](https://img.shields.io/badge/license-Apache-blue.svg)](./LICENSE.txt)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Learn how to instrument your BattleSnake with New Relic using the NodeJS agent.
For this repository we are using [BattleSnake JavaScript starter](https://github.com/BattlesnakeOfficial/starter-snake-javascript) from the BattleSnake Official.


* [Installation](#installation)
* [Usage](#usage)
    * [Customizing The App](#customizing-the-app)
    * [Deploying to Heroku](#deploying-to-heroku)
* [Support](#support)
* [License](#license)


## Intrumentation
- [Create a free account at New Relic](https://newrelic.com/signup?utm_source=devrel&utm_medium=organic_social&utm_campaign=github_newrelic_experimental_devrel_repo),
- On the New Relic One home page, select the + Add more data button on the top right, and choose Node.js under App Monitoring,
- On the next page click on Begin instalation and choose how you will be installing your Node.js agent, here we are using a Package Manager,
- Name your application,
- On your cloned or forked repository, first change into the directory and execute the following commands in your terminal to install the agent:

```bash
 npm install newrelic --save
```
- Download the custom configuration file, and add it to the root of your Node.js application,
- Add New Relic to your applicatio's main mmodule, pasting the cfollowing command on the first line of your app's main module:
```bash
 require('newrelic');
```
- Start your application and as soon as it is running, New Relic is collecting your BattleSnake data.


### Deploying to Heroku

You can deploy the application directly from this GitHub repository by clicking on the `Deploy to Heroku` button at the top of this README. Once you do that you still must set your New Relic License key in Heroku. You can either do so at the time you are initializing your application after you have the clicked the `Deploy to Heroku` button above, or after from within the Heroku Dashboard.

After you have clicked the above `Deploy to Heroku` button, you will see one option for the `config vars` in the Heroku deployment settings. Add your New Relic License Key before clicking the final `Deploy app` button. This will ensure your application is deployed to Heroku with your information.

Alternatively, you can do so from with your Heroku Dashboard's application settings by [managing the config vars](https://devcenter.heroku.com/articles/config-vars#using-the-heroku-dashboard) for your Phoenix app after deploying. You will need to add the environment variable: `NEW_RELIC_LICENSE_KEY`.

## Support

New Relic has open-sourced this project. This project is provided AS-IS WITHOUT WARRANTY OR DEDICATED SUPPORT. Issues and contributions should be reported to the project here on GitHub.

We encourage you to bring your experiences and questions to the [Explorers Hub](https://discuss.newrelic.com) where our community members collaborate on solutions and new ideas.

## Contributing

We encourage your contributions to improve this demo app! Keep in mind when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. You only have to sign the CLA one time per project. If you have any questions, or to execute our corporate CLA, required if your contribution is on behalf of a company, please drop us an email at opensource@newrelic.com.

**A note about vulnerabilities**

As noted in our [security policy](../../security/policy), New Relic is committed to the privacy and security of our customers and their data. We believe that providing coordinated disclosure by security researchers and engaging with the security community are important means to achieve our security goals.

If you believe you have found a security vulnerability in this project or any of New Relic's products or websites, we welcome and greatly appreciate you reporting it to New Relic through [HackerOne](https://hackerone.com/newrelic).

## License

This project is licensed under the [Apache 2.0](http://apache.org/licenses/LICENSE-2.0.txt) License.

[license]: LICENSE.md

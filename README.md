#  browserstack-gradle-testng-appium
This repo contains samples for running Appium tests with TestNG, in Gradle subprojects, using the BrowserStack SDK.

## Setup
* Clone the repo `git clone https://github.com/Roger-BStack/browserstack-gradle-testng-appium.git`
* Set credentials in the `BROWSERSTACK_USERNAME` and `BROWSERSTACK_ACCESS_KEY` environment variables (see below for details), or update credentials in the `browserstack.yml` file with your [BrowserStack Username and Access Key](https://www.browserstack.com/accounts/settings).

## Running tests:
* To run only the sample tests, ofr Android and iOS, on BrowserStack, run `gradlew clean test`.
* To run All the tests on BrowserStack, including BrowserStack Local Sample Tests, run `gradlew clean mobiletests`.
* To run the Android sample test on BrowserStack, run `gradlew clean :android:sampleTest`.
* To run the iOS sample test on BrowserStack, run `gradlew clean :ios:sampleTest`.

Understand how many parallel sessions you need by using our [Parallel Test Calculator](https://www.browserstack.com/automate/parallel-calculator?ref=github)

## Notes
* You can view your test results on the [BrowserStack Automate dashboard](https://www.browserstack.com/automate)
* You can export the environment variables for the Username and Access Key of your BrowserStack account.

    * For Unix-like or Mac machines:
  ```
  export BROWSERSTACK_USERNAME=<browserstack-username> &&
  export BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
  ```

    * For Windows:
  ```
  set BROWSERSTACK_USERNAME=<browserstack-username>
  set BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
  ```
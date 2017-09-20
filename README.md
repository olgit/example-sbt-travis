# Black Duck CoPilot Scala Build Tool/Travis CI Example

[![Travis CI](https://travis-ci.org/BlackDuckCoPilot/example-sbt-travis.svg?branch=master)](https://travis-ci.org/BlackDuckCoPilot/example-sbt-travis) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/groups/BlackDuckCoPilot/locations/example-sbt-travis/public/results/branches/master/badge-risk.svg)](https://copilot.blackducksoftware.com/github/groups/BlackDuckCoPilot/locations/example-sbt-travis/public/results/branches/master)

Shows a working setup for using Black Duck CoPilot to analyze the risk of project dependencies

## Travis CI Setup

The `.travis.yml` file has been modified to upload the generated data to Black Duck CoPilot:

```yaml
after_success:
  - bash <(curl -s https://copilot.blackducksoftware.com/ci/travis/scripts/upload)
```

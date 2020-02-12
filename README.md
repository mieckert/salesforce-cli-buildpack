# Heroku Buildpack for Salesforce CLI (SFDX) and more

This a Heroku Buildpack installing Salesforce CLI (SFDX), several plug-ins, jq (and potentially more)
into your Heroku Dyno.  It is a fork from Shane's fork of the Heroku Buildpack.

## Usage

To use `sfdx`, you simply need to export the appropriate paths:

```
export PATH="$BUILD_DIR/vendor/sfdx/cli/bin:$PATH"
```

The `$BUILD_DIR` is the path where your apps source is stored on the Heroku dyno.
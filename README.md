# OpenShift NewRelic Agent Cartridge

The `newrelic-agent` cartridge provides [NewRelic](http://www.newrelic.com/) agent for PHP applications, to install create your app and run:

	rhc add-cartridge http://reflector-getupcloud.getup.io/reflect?github=getupcloud/openshift-newrelic-php-agent --app [APP]

## Configuration 

The newrelic agent install the php module and configures the cartridge to push metric to newrelic servers. All you need to do is set the `OPENSHIFT_NEWRELIC_LICENSE_KEY` environment variable and restart the app.

	rhc set-env  OPENSHIFT_NEWRELIC_LICENSE_KEY=PUT_YOUR_LICENSE_HERE -a [APP]
	rhc app-restart [APP]

# Important!

This cartridge was designed to work on Getup Cloud Openshift and may not work on your installation, use at your own risk.

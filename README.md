# TAURUS Let's test

## Proc pouzivat Taurus
- wrapper nad JMeter, Gatlingem a dalsimi
- umoznuje definovat konfiguracni soubory v yaml
- pretezuje nastaveni TP
- Building JMeter TP v YAML https://gettaurus.org/docs/JMeter/#Building-Test-Plan-from-Config


## Poznamky
- Taurus supports running more than one existing JMeter .jmx test script from a YAML file as well
- Add (or override) any property (including JMeter properties and system properties).
- Add (or override) user-defined variables.
- Enable/Disable any test element starting from the Thread Group and ending up with listeners.
- Taurus domain specific language (DSL) written in either JSON or YAML allows you to generate scripts in JMeter, Grinder, or Gatling and to override the settings of existing scripts written for those tools.


## TODO
- JMeter Executor (https://gettaurus.org/docs/JMeter/#Building-Test-Plan-from-Config)
- Logging to Elastic

## Runner
```
docker run -it --rm -v `pwd`/tests:/bzt-configs blazemeter/taurus my-config.yml -o modules.console.disable=true
```
# Hass.io Add-on: Signal Messenger

This project provides a Hass.io addon around [signal-cli-rest-api](signal-cli-rest-api) for use with the [Signal Messenger integration](https://www.home-assistant.io/integrations/signal_messenger/)

On first startup you will need to register a number, and verify it with the SMS code.
If you use all the defaults, then something like the following should get things set up.

```sh
curl -X POST -H "Content-Type: application/json" \
    'http://hassio:8080/v1/register/+61234567890'

curl -X POST -H "Content-Type: application/json" \
    'http://hassio:8080/v1/register/+61234567890/verify/123-456'
```

# Ecowater water softeners integration for Home Assistant

[![Validate with HACS](https://github.com/ThePrincelle/homeassistant-ecowater-softener/actions/workflows/validate-hacs.yml/badge.svg)](https://github.com/ThePrincelle/homeassistant-ecowater-softener/actions/workflows/validate-hacs.yml)
[![Validate with hassfest](https://github.com/ThePrincelle/homeassistant-ecowater-softener/actions/workflows/validate-with-hassfest.yml/badge.svg)](https://github.com/ThePrincelle/homeassistant-ecowater-softener/actions/workflows/validate-with-hassfest.yml)

`ecowater_softener` is a _custom component_ for [Home Assistant](https://www.home-assistant.io/). The integration allows you to pull data from your Ecowater water softener.

It will create one sensor with multiple attributes.

![Homeassistant sensor more info dialog](attributes.png)

## Installation

#### HACS

#### Manually
Copy the `custom_components/ecowater_softener` folder into the config folder.

## Configuration
To add an Ecowater water softener, go to Configuration > Integrations in the UI. Then click the + button and from the list of integrations select Ecowater Softener. You should then see a dialog like the one below.

![Ecowater custom component setup dialog](setup.png)

You then need to enter the information you use to login on [https://wifi.ecowater.com/Site/Login](https://wifi.ecowater.com/Site/Login). (Serial Number = DSN)

Then you will need to select the date format that your Ecowater device uses. You can check this under the `Out of Salt Date` and `Last Recharge` at [https://wifi.ecowater.com/Site/Login](https://wifi.ecowater.com/Site/Login).

This will then create an entity `sensor.ecowater_serialnumberhere`. This sensor will update every 30 minutes.

## License
[MIT](https://choosealicense.com/licenses/mit/)

# UniFi LED API

This is an _unofficial_ (and incomplete) documentation to control UniFi LED panels throug REST API.

## Motivation
[UniFi Network-Managed LED Panel and Dimmer Switch](https://unifi-led.ui.com/) are very good solutions for POE lighting. Unluckily, at the moment the only official ways to control the lights are through the [EOT Led Controller](https://github.com/ubiquiti/eot-controller) or the UniFi LED mobile app ([Android](https://play.google.com/store/apps/details?id=com.ubnt.unifi.official&hl=it), [Apple Store](https://apps.apple.com/us/app/unifi-led/id1384397383)).

However, with a bit of work we were able to understand how the API works and control the lights programmatically. This repository is intended to help other people with the same needs to achieve this result!

## State of the art
With the API documented in this repository you can turn on and off single lights and groups of lights, dimmer the lights, obtain tokens (having the controller username and password).

Please note that you the API communicates with the LED controller, _not_ directly with the LED panels. That is, you have to have the EOT LED Controller up and running to use this API.

## Prerequisites
This APIs are tested in the following scenario:
- ULED-AT
- EOT LED Controller v1.6.1 BETA

## Postman collection
The REST API reference is published also in [this page](https://documenter.getpostman.com/view/1477209/SWT7BKDA?version=latest) on the Postman documenter website.

## Node-RED
We also created a [Node-RED flow](node-red/flow.json) to control the lights, adding some nice effects.





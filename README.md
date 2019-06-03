# mikrotik-cloudflare-ddns-scripts

This simple scripts are designed to implement `DDNS` feature using the service [Cloudflare](https://www.cloudflare.com/).

### Requirements and dependences

Scripts work only on `RouterOS` version 6.44 and above.

Depends on [Mikrotik JSON Parser](https://github.com/Winand/mikrotik-json-parser) project installed as system script with name `JParseFunctions`.

### Configure

Each script (IPv4 and IPv6) has a configuration area. Just insert your values.

First of all you need your `Cloudflare API` key. Just go to the `Cloudflare` [site](https://www.cloudflare.com/) `My Profile -> API Keys section -> Global API Key -> View`. Follow the instructions. Now you have your `API` key. Keep it safe.

The service does not allow easy retrieval of required DNS record identifiers. This is only possible through a REST API method `List DNS Records`. This method is described [here](https://api.cloudflare.com/#dns-records-for-a-zone-list-dns-records). Using any REST client (I use [Advanced REST client](https://chrome.google.com/webstore/detail/advanced-rest-client/hgmloofddffdnphfgcellkdfbfbjeloo) for `Chrome Browser`), sending a request, you will receive the `JSON` answer with necessary zone and host IDs.

Insert all variables in scripts and install in your `Mikrotik` device.

### Running

You may add this script to system scheduler as periodically task.

#### Thanks for using.

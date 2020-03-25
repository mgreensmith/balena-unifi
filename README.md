## Unifi Controller on Balena

Deployment repo for a Unifi Controller container into a Balena application (RasPi 3).

### Usage notes:
- Set a static IP reservation on the router for the MAC of the device (or configure a static IP in balenaOS).
- If using an EdgeRouter, set the `Unifi Controller` address in the DHCP server to the IP of the device.
- Before adopting any Unifi devices, you must configure the Inform Host statically, because the controller does not know its own IP.
	- `Unifi Controller` > `Settings` > `Controller Settings` > `Advanced Configuration`
		- *Controller Hostname/IP:* Set to the IP of the device.
		- *Override Inform Host with Controller Hostname/IP:* Enable this.

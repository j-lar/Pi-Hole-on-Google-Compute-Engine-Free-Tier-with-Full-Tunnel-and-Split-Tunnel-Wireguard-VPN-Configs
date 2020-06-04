# Common Wireguard VPN Client Configuration Steps

At the end of the Quickstart or Detailed Server Setup Guide, a Wireguard configuration file named **wg0-client-1.conf** should have been created. This allows a client to connect to the VPN. A visual representation of the **wg0-client-1.conf** configuration file also appears as a QR Code, and the VPN Profile can be scanned using the Android or iOS Wireguard apps.

If you are setting up a Wireguard Client on a computer or server, obtain the contents of the **wg0-client-1.conf** file and copy it to the device you want to connect from.

You can print the contents of the **wg0-client-1.conf** file in the command line interface of the Wireguard Server, by running this command:

```bash
sudo cat /root/wg0-client-1.conf
```

The output can be copy and pasted into a blank text file on your client device, and this configuration file should be saved on your client device with a **.conf** suffix.

---

## Android

<a href="https://f-droid.org/en/packages/com.wireguard.android/" target="_blank">
<img src="./images/logos/f-droid.svg" alt="Get it on F-Droid" height="80"></a>
<a href="https://play.google.com/store/apps/details?id=com.wireguard.android" target="_blank">
<img src="./images/logos/google-play.svg" alt="Get it on Google Play" height="60"></a>

## Arch Linux

### 1. Install Wireguard plugin

As a prerequisite, you should have the [Wireguard plugin for Network Manager](https://github.com/max-moser/network-manager-wireguard/) installed.

From the Arch User Repository, you can install **networkmanager-wireguard-git**.

### 2. Import the configuration

  1. Right click on Network Manager applet
  2. Select **Modify connections**
  3. At the bottom left, click on the `+` symbol
  4. From the dropdown menu, select **Import saved VPN configuration** and confirm
  5. Select the **wg0-client-1.conf** file and confirm.
  6. You are free to change the name of the VPN configuration if you want. Once done, click **Save** and you should see the VPN connection appear in the list.

## iOS

<a href="https://itunes.apple.com/us/app/wireguard/id1441195209?ls=1&mt=8" target="_blank">
<img src="./images/logos/app-store.svg" alt="Get it on the App Store" height="60"></a>

## macOS

<a href="https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1&mt=12" target="_blank">
<img src="./images/logos/app-store-macOS.svg" alt="Get it on the Mac App Store" height="60"></a>

## Windows

Get the latest Windows Client from [wireguard.com/install](https://www.wireguard.com/install/)
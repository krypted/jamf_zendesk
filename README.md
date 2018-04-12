# Jamf|Pro Zendesk Sidebar App

This Zendesk sidebar app gathers device information from Jamf Pro based on email from submitted ticket.


### Setup:

* Upload the .zip to your Private Apps section of Zendesk
* In the App Configuration settings ensure you supply:
- Your domain or FQDN (yourcompany.jamfcloud.com or servername.yourcompany.com)
- Your full Jamf Pro URL (https://yourcompany.jamfcloud.com or https://servername.yourcompany.com:8443)
- Base64 token without parenthesis (username:password)
- (for macOS users) 3 extension attribute Jamf IDs for macOS devices


### The following information is displayed:

* If an iOS or macOS device is found based on email in ticket and email assigned in Jamf Pro, the device information will display in the sidebar.
* If no devices or multiple devices are found, you will be prompted with a search bar to gather information based on a chosen search term and dropdown list.

macOS:
- Assigned User
- Computer Name
- Serial Number
- Last Check-in
- Custom Extension Attribute 1
- Custom Extension Attribute 2
- Custom Extension Attribute 3

iOS:
- Assigned User
- iOS Device Name
- iOS Device Type
- Serial Number
- Last Check-in

Please submit bug reports to [Issues](https://github.com/krypted/jamf_zendesk/issues). Pull requests are welcome.

- On-prem and Jamfcloud users!
- Parses Zendesk ticket for email used to create ticket
- Uses that email to find assigned devices in Jamf Pro
- If either a macOS or iOS device is found, data will show in sidebar
- If user has multiple devices, a hotlink taking you to that user in Jamf Pro will show. Along with a quick search tool to GET a return from Jamf Pro API.
- For macOS, in App Settings in Zendesk, you can add the ID's of 3 extension attributes to gather more information that is not default

### Screenshot(s):
![Screenshots](https://github.com/krypted/jamf_zendesk/blob/master/Screenshots.png)

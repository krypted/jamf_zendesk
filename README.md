# Jamf|Pro Zendesk Sidebar App

This Zendesk sidebar app gathers device information from Jamf Pro based on email from submitted ticket.

### The following information is displayed:

* In the App Configuration settings ensure you supply your Jamfcloud instance name, base64 token, and 3 extension attribute Jamf IDs for macOS devices.
* If no devices or multiple devices are found, you will be prompted with a search bar to gather information based on a chosen search term and dropdown list.
* If an iOS or macOS device is found based on email in ticket and email assigned in Jamf Pro, the device information will display in the sidebar.

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

### Setup:

- Jamfcloud users only (at this time)
- Parses Zendesk ticket for email used to create ticket
- Uses that email to find assigned devices in Jamf Pro
- If either a macOS or iOS device is found, data will show in sidebar
- If user has multiple devices, a hotlink taking you to that user in Jamf Pro will show. Along with a quick search tool to GET a return from Jamf Pro API.
- For macOS, in App Settings in Zendesk, you can add the ID's of 3 extension attributes to gather more information that is not default

### Screenshot(s):
![Screenshots](https://github.com/krypted/jamf_zendesk/blob/master/Screenshots.png)

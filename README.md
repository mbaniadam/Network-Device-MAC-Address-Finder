## Network Device MAC Address Finder
This Python script helps you find the MAC address of a target IP address across multiple network devices. It uses the Netmiko library for SSH connectivity and automation tasks on network devices.

### Prerequisites
Before using this script, make sure you have the following prerequisites:

- Python 3.x installed.
- The netmiko library installed. You can install it using pip:
```console
pip install netmiko
```

### Usage

Clone this repository to your local machine or download the script directly.

Create a JSON file named hosts.json in the same directory as the script. This JSON file should contain a list of network device IP addresses or hostnames that you want to search for the MAC address. For example:

```console
[
    "192.168.1.1",
    "192.168.1.2",
    "switch.example.com"
]
```
Run the script by executing the following command in your terminal:
```console
python network_mac_finder.py
```

Follow the on-screen prompts:

Enter your username and password when prompted.
Enter the target IP address for which you want to find the MAC address.
The script will then attempt to connect to the specified network devices, retrieve MAC address information, and display the results. If a MAC address is found, it will display the MAC address and additional information about the interface where the MAC address is located. If a MAC address is not found on a device, it will indicate that.

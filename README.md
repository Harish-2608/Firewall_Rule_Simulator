# Firewall_Rule_Simulator

This project is a simple Python program that simulates firewall rules and random IP traffic generation. The program checks each randomly generated IP address against a set of predefined firewall rules and determines whether the IP should be "allowed" or "blocked."

## Features

- **Random IP Generation**: IPs are randomly generated in the format `192.168.1.X`, where `X` is a random number between 0 and 225.
- **Firewall Rules**: The program checks if the generated IP matches any predefined rules. If a match is found, the specified action (`block` or `allow`) is returned.
- **Customizable Rules**: The firewall rules can be easily modified in the code.
- **Random Number Generator**: Along with the firewall check, the program generates a random ID (1111-9999) for each simulated IP request.

## Code Overview

1. **`generate_random_ip()`**:
   - Generates a random IP address in the range `192.168.1.0` to `192.168.1.225`.

2. **`check_firewall_rules(ip, rules)`**:
   - Checks if the generated IP matches any of the firewall rules. If it does, the corresponding action is returned. If no match is found, the default action is "allow."

3. **`main()`**:
   - Defines the firewall rules and simulates 20 network traffic events. For each event, a random IP is generated, checked against the rules, and a ID is also generated for additional output.

## Example Output
- IP: 192.168.1.17, Action: allow, ID: 3729 
- IP: 192.168.1.4, Action: block, ID: 9321 
- IP: 192.168.1.11, Action: allow, ID: 1222
- IP: 192.168.1.9, Action: block, ID: 1198 

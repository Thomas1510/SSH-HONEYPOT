# SSH Honeypot Project

## Overview

The **SSH Honeypot** is a security project designed to emulate an SSH service in order to attract and monitor unauthorized login attempts. By deploying this honeypot, you can capture and analyze malicious activity targeting SSH servers, such as brute-force attacks, credential harvesting attempts, and other malicious actions. This project provides a controlled environment for researchers and cybersecurity professionals to study attack patterns and improve defense strategies.

## Features

- **Emulated SSH Service**: The honeypot simulates a real SSH server and listens for incoming connections from attackers.
- **Log Malicious Attempts**: All login attempts, including successful and failed ones, are logged for further analysis.
- **No Geolocation or Fake Environment**: The honeypot does not simulate fake geolocation or environment details, ensuring that any attacker interacting with it sees the environment as realistic as possible.
- **Customizable User and Password Authentication**: The honeypot allows any user and password combination to connect, increasing the likelihood of attracting attackers who use automated scripts.
- **Network Traffic Analysis**: Capture network traffic to analyze patterns of attack and identify common tactics used by malicious actors.

## Advantages

- **Realistic SSH Service**: By providing an open, unmonitored SSH port, the honeypot can attract real-world attackers, helping you gather valuable threat intelligence.
- **Easy to Deploy**: The honeypot can be set up and run quickly on any machine that supports Python and SSH.
- **No Risk to Production Systems**: Since the honeypot is isolated from the rest of your infrastructure, attackers are confined to a controlled environment.
- **Useful for Research**: Security professionals and researchers can use the data from the honeypot to study attack patterns and develop better defense mechanisms.
- **Customizable**: Easily modify the honeypot’s behavior, such as adding more fake login prompts or tweaking logging mechanisms, to suit your specific research needs.

## Requirements

- Python 3.x or higher
- No additional external libraries required (built using standard Python libraries)

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/your-username/ssh-honeypot.git
    ```

2. Navigate to the project directory:

    ```bash
    cd ssh-honeypot
    ```

3. Install any necessary dependencies (if applicable):

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Running the Honeypot

1. In the terminal, navigate to the folder where the honeypot script is located.
2. Run the honeypot script:

    ```bash
    python ssh_honeypot.py
    ```

3. The honeypot will start, and you will begin to see log entries of incoming SSH connection attempts.

### Viewing Logs

1. Check the logs in the `logs/` directory for a detailed record of attempted SSH connections, including usernames, passwords, IP addresses, and timestamps.
2. Analyze these logs to study attack patterns, identify vulnerable credentials, and assess the behavior of attackers.

## Contributing

Feel free to fork the repository, submit issues, and create pull requests. If you'd like to contribute, please follow best practices in Python and cybersecurity, keeping the code clean, well-documented, and secure.

## Disclaimer

This project is intended solely for educational and research purposes. Do not use this honeypot on production systems or networks without proper security measures and monitoring.


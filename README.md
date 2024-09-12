# Secure VPN Configuration for Remote Access

![VPN Setup Diagram]![image](https://github.com/user-attachments/assets/a8714cae-65e8-43a9-a1e8-3aad27d75144)

)
)

## Introduction

In this project, I configured two travel routers—**Flint 2** and **Beryl AX GL-MT3000**—to establish a secure VPN connection to my home network. The goal was to ensure secure, encrypted access to network resources while traveling. The VPN setup prioritizes security and ensures that user privacy and sensitive data are safeguarded during remote sessions. Both **OpenVPN** and **WireGuard** protocols were implemented for secure tunneling, along with firewall configurations and private endpoints for additional protection.

## Architecture
The architecture of this VPN project consists of:

- **Flint 2 Router**
- **Beryl AX GL-MT3000 Travel Router**
- **OpenVPN / WireGuard** for secure tunneling
- **Home VPN Server** for secure remote access
- **Firewall Rules** for network security
- **Private Endpoints** to protect resources

### VPN Setup:
1. **OpenVPN Configuration**: Setup and configure OpenVPN on Flint 2 and Beryl AX routers, establishing a secure tunnel between the remote user and the home network.
2. **WireGuard Setup**: Configured WireGuard as an alternative lightweight VPN solution for faster connection speeds and low latency.
3. **Home VPN Server**: Deployed a home VPN server to manage VPN connections and ensure secure access to network resources.
4. **Firewall Configurations**: Hardened firewall settings by restricting access to only trusted IP addresses, preventing unauthorized connections.
5. **Private Endpoints**: Applied Private Endpoints for further securing sensitive network resources from public exposure.

## Secure VPN Configuration Workflow

### Step 1: Flint 2 Router Configuration
- **OpenVPN Setup**: Configured OpenVPN on Flint 2 for encrypted tunneling.
- **Firewall Rules**: Implemented firewall rules to allow only trusted IP addresses.
- **WireGuard Setup**: Deployed WireGuard as a fast VPN alternative for secure connections.

### Step 2: Beryl AX GL-MT3000 Router Setup
- **Secure Travel Router Setup**: Configured Beryl AX GL-MT3000 for remote access while traveling, using both OpenVPN and WireGuard protocols.
- **MDM and VPN Client**: Integrated Mobile Device Management (MDM) and set up VPN clients for remote devices to securely connect to the home VPN.

### Step 3: Testing and Validation
- **Connection Tests**: Validated the secure VPN connection by accessing network resources remotely through both VPN protocols.
- **Performance Evaluation**: Monitored and compared the performance of OpenVPN and WireGuard.
- **Security Check**: Reviewed firewall and VPN logs to confirm encrypted connections and ensure data security.

## Metrics Before Hardening / Security Controls
Before hardening, the VPN setup allowed broad access with minimal restrictions. The metrics observed before applying firewall rules and IP restrictions were as follows:

| Metric                    | Result |
| ------------------------- | ------ |
| Encrypted Connections      | 100%   |
| Unauthorized Access Alerts | 5      |
| Ping Response Time         | 120ms  |
| VPN Throughput (OpenVPN)   | 30Mbps |
| VPN Throughput (WireGuard) | 50Mbps |

## Metrics After Hardening / Security Controls
After applying strict firewall rules and IP-based access control, the VPN setup was significantly more secure, with the following performance metrics:

| Metric                    | Result |
| ------------------------- | ------ |
| Encrypted Connections      | 100%   |
| Unauthorized Access Alerts | 0      |
| Ping Response Time         | 105ms  |
| VPN Throughput (OpenVPN)   | 28Mbps |
| VPN Throughput (WireGuard) | 47Mbps |

## Conclusion

This project demonstrated the successful configuration of secure VPN connections using the Flint 2 and Beryl AX GL-MT3000 routers, ensuring private, encrypted access to home network resources while traveling. Both **OpenVPN** and **WireGuard** protocols were tested for performance and security, with **WireGuard** proving to be more efficient in terms of speed. The application of firewall rules and IP-based restrictions significantly improved network security by eliminating unauthorized access attempts. This setup is ideal for anyone seeking a secure, portable solution for remote network access.

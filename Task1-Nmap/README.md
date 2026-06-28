# Task 1 - Basic Network Scanning with Nmap

## Objective

The objective of this task is to perform a basic network scan using Nmap to identify open ports and running services on the local machine.

## Tool Used

- Nmap 7.94
- Operating System: macOS

## Command Used

```bash
nmap 127.0.0.1
```

## Scan Results

The scan identified the following open ports:

| Port | Service | Description |
|------|---------|-------------|
| 21 | FTP | File Transfer Protocol |
| 88 | Kerberos | Authentication service |
| 3306 | MySQL | Database service |
| 5000 | UPnP | Universal Plug and Play |
| 5900 | VNC | Remote desktop service |
| 7000 | AFS File Server | File sharing service |
| 8021 | FTP Proxy | FTP proxy service |
| 49153 | Unknown | Dynamic/private port |

## Security Significance

- FTP should be secured because it can expose sensitive files.
- Kerberos is used for secure authentication.
- MySQL databases should not be publicly accessible.
- UPnP should be disabled if not required.
- VNC should use strong passwords and encryption.
- Unknown ports should be investigated if unexpected.

## Conclusion

The Nmap scan successfully identified the open ports and services running on the local machine. This helps security analysts understand the attack surface and identify services that require proper security configurations.

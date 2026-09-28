# Pi-hole

Pi-hole is a network-wide DNS sinkhole that blocks advertisements, trackers, and other unwanted domains before they reach devices on your network.

## Features

- Network-wide ad blocking
- Tracker and telemetry blocking
- DNS-level filtering
- Local DNS management
- Custom allowlists and denylists
- Query logging and statistics
- Web-based administration interface
- Lightweight and self-hosted

## How It Works

Pi-hole operates as a DNS server for your network. When a device makes a DNS request, Pi-hole checks the requested domain against its configured blocklists.

If the domain is blocked, Pi-hole prevents the request from resolving normally. Allowed domains are forwarded to the configured upstream DNS provider.

This allows filtering to work across multiple devices without requiring browser extensions or individual device configuration.

## Benefits

Pi-hole can help reduce:

- Advertisements
- Tracking domains
- Analytics requests
- Telemetry
- Unwanted third-party connections

Because filtering happens at the DNS level, it can work across computers, phones, smart TVs, game consoles, and other network-connected devices.

## Administration

Pi-hole provides a web interface for managing and monitoring the DNS server.

The dashboard provides information such as:

- DNS queries
- Blocked queries
- Frequently requested domains
- Frequently blocked domains
- Client activity
- Configured blocklists
- DNS settings

## Blocklists

Pi-hole uses domain-based blocklists to determine which DNS requests should be blocked.

Additional lists can be added depending on the desired level of filtering. Domains can also be manually added to allowlists or denylists.

## Important Considerations

Pi-hole blocks domains at the DNS level, so it does not inspect or modify the contents of network traffic.

Some applications may use hard-coded DNS servers, encrypted DNS, or other techniques that can bypass DNS-level filtering.

Pi-hole is therefore best considered a network-wide DNS filtering solution rather than a complete replacement for browser-based or application-level blocking.

## Requirements

Pi-hole can run on a variety of systems, including:

- Raspberry Pi
- Linux servers
- Virtual machines
- Containers
- Other supported hardware and operating systems

## Resources

- [Pi-hole Website](https://pi-hole.net/)
- [Pi-hole Documentation](https://docs.pi-hole.net/)
- [Pi-hole GitHub](https://github.com/pi-hole/pi-hole)

## License

Pi-hole is open-source software distributed under its applicable open-source licenses.

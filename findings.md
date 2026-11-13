# DNS Traffic Analysis – Findings

## 1. Objective
To capture and analyze DNS traffic using Wireshark and understand how domain names are translated into IP addresses.

## 2. Tools Used
- Kali Linux
- Wireshark
- dig
- ping

## 3. Domains Investigated
- google.com – Used for a basic DNS resolution test.
- yahoo.com – Used for detailed DNS traffic capture and analysis in Wireshark.


## 4. DNS Analysis

- DNS record type: A (IPv4)
- Transport protocol: UDP
- DNS server IP: fd17:625c:f037:2::3
- Kali Linux IP: fd17:625c:f037:2:69a8:6417:7711:6096
- Source port: 53
- Destination port: 44413
- DNS response code: No error (0)
- Yahoo DNS response: Six IPv4 addresses returned.

## 5. Packet Size Comparison

- DNS query UDP length: 58 bytes
- DNS response UDP length: 142 bytes

The response was larger because it contained multiple DNS answers.

## 6. Key Observations

Wireshark successfully captured DNS queries and responses. The matching transaction ID helped identify the corresponding query and response.

## 7. Conclusion

This project demonstrated how DNS resolves domain names into IP addresses and how Wireshark can be used to inspect DNS traffic, IP addresses, UDP ports, response codes, and packet sizes.

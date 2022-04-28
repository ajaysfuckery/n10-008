# Ethernet/IP Headers
<hr>
#### OSI Layers
- Ethernet -> Layer 2
- IP Header -> Layer 3
- TCP/UDP Header -> Layer 4

<hr>
#### Ethernet Frame Format
| Preamble | SFD | Destination Address | Source Address | Length | Data | CRC |
|---|---|---|---|---|---|---|
	| 7 Bytes | 1 Byte | 6 Bytes | 6 Bytes | 2 Bytes | 46-1500 Bytes | 4 Bytes

<hr>
#### Extended Ethernet Frame (Ethernet II Frame)
| DA | SA | Type | DSAP | SSAP | Ctrl | Data | FCS |
|---|---|---|---|---|---|---|---|
| 6 Bytes | 6 Bytes | 2 Byte | 1 Byte | 1 Byte | 1 Byte | 46 Bytes | 4 Bytes |

<hr>
#### IPv4 Header

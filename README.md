Task 4 – Firewall Setup on Windows

Tool Used
Windows Defender Firewall with Advanced Security (wf.msc)

Rules Applied
| Rule | Port | Protocol | Action |
|------|------|----------|--------|
| Block Telnet | 23 | TCP | BLOCK |
| Allow HTTP | 80 | TCP | ALLOW |

 Test Result
- Ran: Test-NetConnection -ComputerName localhost -Port 23
- Result: TcpTestSucceeded : False (port successfully blocked)

Files
- firewall_backup.wfw – exported firewall config
- firewall_rules.txt – all rules in text format
- screenshots/ – proof of rules and testing


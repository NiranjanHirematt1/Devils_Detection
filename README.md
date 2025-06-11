# Devils_Detection


simple detection engine architecture

main.py
├── sniffer.py           # Captures raw packets (Scapy/pyshark)
├── parser.py            # Extracts source IP, dest IP, ports, protocol, payload
├── signature_engine.py  # Loads rules and performs matching on parsed data
├── rules/
│   └── http_rules.json  # Example rule file (can have more like dns_rules.json, etc.)
├── logger.py            # Logs alerts to detections.log and optionally prints
├── utils.py             # Helper functions (load rules, time formatting, etc.)
└── detections.log       # Output file where alerts are stored

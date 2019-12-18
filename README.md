# device_layer
assistance with device layer troubleshooting

IF-MIB 1.3.6.1.2.1.2
SNMPv2-MIB 1.3.6.1.2.1.1
LLDP-MIB 1.3.6.1.4.1.9.9.23
CDP-MIB 1.0.8802.1.1.2

IF-MIB 1.3.6.1.2.1.2
snmpwalk -v3 -l AuthPriv -a SHA -A MASKED -x AES -X 2MASKED -u <user> <target> 1.3.6.1.2.1.2 |head

SNMPv2-MIB 1.3.6.1.2.1.1
snmpwalk -v3 -l AuthPriv -a SHA -A -x AES -X -u <user> <target> 1.3.6.1.2.1.1 |head

LLDP-MIB 1.3.6.1.4.1.9.9.23
snmpwalk -v3 -l AuthPriv -a SHA -A -x AES -X g -u <user> <target> 1.3.6.1.4.1.9.9.23 |head

CDP-MIB 1.0.8802.1.1.2
snmpwalk -v3 -l AuthPriv -a SHA -A -x AES -X -u <user> <target> 1.0.8802.1.1.2 |head

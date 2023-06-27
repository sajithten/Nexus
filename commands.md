## To enable grace period license:
```
license grace-period
```
## To check ssh enabled:
```
show ssh server
```
## To see enabled features:
```
show feature
```
## To see user accounts:
```
show user-account
```
## To create user & assign role:
```
username <name> password <password> role <role_name>
```
## To create port profile:
```
N7K-01(config)# <role_name> port-profile type ethernet <profile_name>
```
## To apply config to profile:
```
N7K-01(config)# port-profile type ethernet <profile_name>
N7K-01(config-port-prof)# no shutdown
N7K-01(config-port-prof)# switchport mode access
N7K-01(config-port-prof)# switchport access vlan 10
N7K-01(config-port-prof)# spanning-tree port type edge
```
## To check status of profile
```
show port-profile
```
## To enable the profile:
```
N7K-01(config-port-prof)# port-profile type ethernet <profile_name>
N7K-01(config-port-prof)# state enabled
```
## To see VDC:
```
show vdc
```
## To create VDC:
```
configure terminal
vdc <vdc_name>
allocate interface ethernet 2/11
```
## To delete VDC:
```
no vdc <vdc_name>
```
## To configure HA policy in VDC:
```
ha-policy single_sup ?
```
## To see currently attached FEX units:
```
show fex
```
## To verify FEX:
```
show vpc
show vpc peer-keepalive
show port-channel summary
```

                                                               
##  To check status of switch stack members
```
sh switch detail
```
## To check fan, temp of fex 110
```
sh env fex 110 

```
## To check interface state under po102
```
show port-channel summary interface port-channel 102
```

## To cpu usage
```
show processes cpu history sh processes cpu sort | ex 0.0
```
## To clear counter for an interface
```
clear counters interface Ethernet110/1/7 
```
#########################

```
sh fabricpath route switchid 1532
```

```
sh ip route 10.38.72.200 vrf 1:1100
```

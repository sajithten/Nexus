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
To apply config to profile:
```
N7K-01(config)# port-profile type ethernet <profile_name>
N7K-01(config-port-prof)# no shutdown
N7K-01(config-port-prof)# switchport mode access
N7K-01(config-port-prof)# switchport access vlan 10
N7K-01(config-port-prof)# spanning-tree port type edge
```
## To
                                                               
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

---
created: "[[2025-10-02]]"
aliases:
tags:
  - "#zettel"
references:
links:
questions:
share_link: https://share.note.sx/t6v491fb#OYtMK30qSaviRxuF5LikL+mfo9ofGLUFW3LGY4y3rXs
share_updated: 2025-10-03T11:42:48-04:00
---
> [!Summary]
> [[Link Labs]] [[SuperTag]]s report their signal quality parameters, cell RSRP and RSRQ with every uplink, which gives insight into [[LTE-M]] signal quality in the specific location the uplink occurred. 

# Typical Signal Strength Ranges
![[Pasted image 20251003113521.png]]
- RSRQ -13 dB and RSRP -120 dBm is reasonable
- Devices have been seen to connect with -130 dBm RSRP and -19 dB RSRQ, which can be considered edge of link

# Supporting Information 
## References:
https://5gstore.com/blog/2021/04/08/understanding-rssi-rsrp-and-rsrq/?srsltid=AfmBOoq6Xna72vMcXqWCl_GoIW7MBZRyQ5Xg7YOG1Wz-kuu1zNRhsZfe

https://support.cel-fi.com/hc/en-us/articles/1260805036129-Understanding-LTE-Signal-Strength-Values

## Exceptions 
### Downtown Deployments of Symphony Link Gateways
- Very poor RSRQ values paired with excellent RSRP values can be observed
- In these cases Gateway operation is not impeded
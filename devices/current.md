```mermaid
flowchart LR

  onu[ONU\nPR-S300HI]
  phone[Phone\nVE-GP24DW]
  airmac[AirMac Time Capsule]
  switch[Switching Hub\nTL-SG508]
  ps5[PS5]
  nx1[Nintendo Switch 1]
  nx2[Nintendo Switch 2]
  speaker[Soundbar\nYAS-108]
  hikaritv[Hikari TV\nST-4500]
  tv[TV\nREGZA 43M540X]

  onu -- Ethernet --- switch
  onu -- Ethernet --- airmac
  onu -- Ethernet --- tv
  tv -- HDMI --- hikaritv
  onu -- Ethernet --- hikaritv
  onu -- TEL --- phone
  switch -- Ethernet --- ps5
  switch -- Ethernet --- nx1
  switch -- Ethernet --- nx2
  nx2 -- HDMI --- speaker
  tv -- HDMI --- speaker
  tv -- HDMI --- nx1
  tv -- HDMI --- ps5

```

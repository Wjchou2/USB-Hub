# William's USB HUB

A compact custom USB 2.0 hub PCB based on the USB2514B controller. It features two USB-A ports and a 4-pin header breakout for easy integration with embedded systems or custom hardware projects.
Simply use a USB-C to C cable to plug the hub into your computer, and check that the LED indicator is on. Then connect any USB-A devices and they will show up on your computer.
I made this project because I have a Mac and never seem to have enough adapters, I also find that I use 4 pin headers often when tinkering with microcontrollers, so I added an easy access 4 pin header integrated into the hub. 

<img width="782" height="543" alt="Screenshot 2026-01-31 at 4 56 15 PM" src="https://github.com/user-attachments/assets/bbd3fe22-d50d-4d83-bb3a-aaf3e4409bb0" />
<img width="762" height="705" alt="Screenshot 2026-01-31 at 4 55 53 PM" src="https://github.com/user-attachments/assets/4c1286c5-0f7f-4fd4-be42-4f9010c4ccfb" />
<img width="680" height="568" alt="Screenshot 2026-01-31 at 11 14 54 PM" src="https://github.com/user-attachments/assets/021ffeb7-521c-40b4-9cfb-f1daf7cc5e32" />
<img width="700" height="537" alt="Screenshot 2026-01-31 at 11 34 22 PM" src="https://github.com/user-attachments/assets/6395f689-9fdb-41e8-93a1-00ad4e8a42ae" />

BOM:
| Designator  | Footprint                                               | Quantity | Designation                 | Link                                                                                                       | Cost   | Total Cost |
|-------------|---------------------------------------------------------|----------|-----------------------------|------------------------------------------------------------------------------------------------------------|--------|------------|
| U2          | SOT-223                                                 | 1        | AMS1117-3.3                 | https://www.lcsc.com/product-detail/C6186.html?s_z=n_AMS1117-3.3                                           | 0.1876 | 0.1876     |
| R3          | R_0603_1608Metric_Pad0.98x0.95mm_HandSolder             | 1        | 12k                         | https://www.lcsc.com/product-detail/C2906989.html?s_z=n_12k%25201%2525%25200603                            | 0.001  | 0.001      |
| R7,R6,R8,R9 | R_0603_1608Metric_Pad0.98x0.95mm_HandSolder             | 4        | 10k                         | https://www.lcsc.com/product-detail/C98220.html?s_z=n_10k%25201%2525%25200603                              | 0.0013 | 0.0052     |
| J2,J3       | USB_A_Receptacle_GCT_USB1046                            | 2        | USB_A                       | https://www.lcsc.com/product-detail/C6307429.html?s_z=n_USB1046                                            | 1.1405 | 2.281      |
| C2,C1,C7    | C_0805_2012Metric_Pad1.18x1.45mm_HandSolder             | 3        | 0.1µ                        | https://www.lcsc.com/product-detail/C53084456.html?s_z=n_100%2520nF%252050V%2520X7R%25200805               | 0.0018 | 0.0054     |
| C4,C3       | C_0603_1608Metric_Pad1.08x0.95mm_HandSolder             | 2        | 22 pF                       | https://www.lcsc.com/product-detail/C695385.html?s_z=n_22%2520pF%2520NPO%25200603                          | 0.051  | 0.102      |
| Y1          | Crystal_SMD_3225-4Pin_3.2x2.5mm                         | 1        | 12.000 MHz                  | https://www.lcsc.com/product-detail/C1647.html?s_z=n_18%2520pF%2520crysta                                  | 0.3272 | 0.3272     |
| J5          | PinHeader_1x04_P2.54mm_Vertical                         | 1        | Conn_01x04_Socket           | https://www.lcsc.com/product-detail/C52016392.html?s_z=n_Pin%2520Header%25201x04%25202.54mm                | 0.0171 | 0.0171     |
| R2,R1       | R_0603_1608Metric_Pad0.98x0.95mm_HandSolder             | 2        | 5.1k                        | https://www.lcsc.com/search?q=5.1k%25201%2525%25200603&s_z=n_5.1k%25201%2525%25200603                      | 0.0012 | 0.0024     |
| R4,R5       | R_0603_1608Metric_Pad0.98x0.95mm_HandSolder             | 2        | 100k                        | https://www.lcsc.com/product-detail/C14675.html?s_z=n_100k%25201%2525%25200603                             | 0.0013 | 0.0026     |
| C6,C5       | C_1206_3216Metric_Pad1.33x1.80mm_HandSolder             | 2        | 10 µF                       | https://www.lcsc.com/product-detail/C342827.html?s_z=n_10%2520uF%252016V%2520X7R%25201206                  | 0.0897 | 0.1794     |
| F1          | Fuse_1812_4532Metric_Pad1.30x3.40mm_HandSolder          | 1        | 0.5A                        | https://www.lcsc.com/product-detail/C7542969.html?s_z=n_PTC%2520fuse%25200.5A%25201812                     | 0.0403 | 0.0403     |
| J1          | USB_C_Receptacle_GCT_USB4105-xx-A_16P_TopMnt_Horizontal | 1        | USB_C_Receptacle_USB2.0_16P | https://www.lcsc.com/product-detail/C2988369.html?s_z=n_USB%2520C%2520receptacle%252016P%2520top%2520mount | 0.0829 | 0.0829     |
| U1          | QFN-36-1EP_6x6mm_P0.5mm_EP3.7x3.7mm                     | 1        | USB2514B_Bi                 | https://www.lcsc.com/product-detail/C220807.html?s_z=n_USB2514B%2520USB%2520hub%25204-port%2520Octopart    | 2.7952 | 2.7952     |
| R10         | R_0603_1608Metric_Pad0.98x0.95mm_HandSolder             | 1        | 1.5kΩ                       | https://www.lcsc.com/product-detail/C22843.html?s_z=n_1.5k%25201%2525%25200603                             | 0.0012 | 0.0012     |
| D1          | LED_0201_0603Metric_Pad0.64x0.40mm_HandSolder           | 1        | LED                         | https://www.lcsc.com/search?q=LED%25200603%2520Green&s_z=n_LED%25200603%2520Green                          | 0.0667 | 0.0667     |
|             |                                                         |          |                             |                                                                                                            |        | 6.0972     |

# 1. Pinout table


<table>
   <tr>
   <td>Peripheral</td><td>Function</td><td>Pin name</td><td>Pin No.</td><td>Comment</td></tr>
   <tr>
   <td rowspan="4">Motor-1</td>
   <td>STEP</td><td>PD4</td><td>85</td><td rowspan="20">All the GPIO related to stepper are converted to 5V output to driver (including STEP, DIR, EN, CS/UART, TMC SPI)</td>
   <tr>
   <td>DIR</td><td>PD3</td><td>84</td></tr>
   <tr>
   <td>EN</td><td>PD6</td><td>87</td></tr>
   <tr>
   <td>CS/UART</td><td>PD5</td><td>86</td></tr>
   <tr>
   <td rowspan="4">Motor-2</td>
   <td>STEP</td><td>PA15</td><td>77</td></tr>
   <tr>
   <td>DIR</td><td>PA8</td><td>67</td></tr>
   <tr>
   <td>EN</td><td>PD1</td><td>82</td></tr>
   <tr>
   <td>CS/UART</td><td>PD0</td><td>81</td></tr>
   <tr>
   <td rowspan="4">Motor-3</td>
   <td>STEP</td><td>PE2</td><td>1</td></tr>
   <tr>
   <td>DIR</td><td>PE3</td><td>2</td></tr>
   <tr>
   <td>EN</td><td>PE0</td><td>97</td></tr>
   <tr>
   <td>CS/UART</td><td>PE1</td><td>98</td></tr>
   <tr>
   <td rowspan="4">Motor-4</td>
   <td>STEP</td><td>PD15</td><td>62</td></tr>
   <tr>
   <td>DIR</td><td>PD14</td><td>61</td></tr>
   <tr>
   <td>EN</td><td>PC7</td><td>64</td></tr>
   <tr>
   <td>CS/UART</td><td>PC6</td><td>63</td></tr>
   <tr>
   <td rowspan="4">Motor-5</td>
   <td>STEP</td><td>PD11</td><td>58</td></tr>
   <tr>
   <td>DIR</td><td>PD10</td><td>57</td></tr>
   <tr>
   <td>EN</td><td>PD13</td><td>60</td></tr>
   <tr>
   <td>CS/UART</td><td>PD12</td><td>59</td></tr>
   <tr>
   <td rowspan="3">TMC SPI</td>
   <td>MISO</td><td>PE13</td><td>66</td><td rowspan="3">LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td>
   <tr>
   <td>MOSI</td><td>PE14</td><td>67</td></tr>
   <tr>
   <td>SCK</td><td>PE12</td><td>65</td></tr>
   <tr>
   <td rowspan="2">Heater</td>
   <td>E0</td><td>PB3</td><td>89</td><td rowspan="2">is converted to 5V to MOSFET with flyback protection</td>
   <tr>
   <td>E1</td><td>PB4</td><td>90</td></tr>
   <tr>
   <tr><td rowspan="3">Temperature</td>
   <td>TH0</td><td>PA2</td><td>24</td><td rowspan="2">4.7KOhm 0.1% pull up resistor for NTC100K,etc. 2.2KOhm 0.1% pull up resistor for PT1000 by jumper. with thermistor protection circuit</td>
   <tr>
   <td>TH1</td><td>PA3</td><td>25</td></tr>
   <tr>
   <td>THB</td><td>PA1</td><td>23</td><td>with thermistor protection circuit</td></tr>
   <tr><td rowspan="5">Endstop</td>
   <td>M1-STOP</td><td>PC1</td><td>16</td><td rowspan="5">Share with M*-DIAG, And high level exceeding 5V are clamped to 5V by diodes</td>
   <tr>
   <td>M2-STOP</td><td>PC3</td><td>18</td></tr>
   <tr>
   <td>M3-STOP</td><td>PC0</td><td>15</td></tr>
   <tr>
   <td>M4-DET</td><td>PC2</td><td>17</td></tr>
   <tr>
   <td>M5-DET</td><td>PA0</td><td>22</td></tr>
   <td rowspan="3">2 wire FAN</td>
   <td>FAN0</td><td>PB7</td><td>93</td><td rowspan="3">is converted to 5V to MOSFET with flyback protection</td>
   <tr>
   <td>FAN1</td><td>PB6</td><td>92</td></tr>
   <tr>
   <td>FAN2</td><td>PB5</td><td>91</td></tr>
   <tr>
   <td rowspan="3">Misc</td>
   <td>RGB1(Neopixel/WS2812)</td><td>PE6</td><td>5</td><td rowspan="1">is converted to 5V</td>
   <tr>
   <td>PS-ON</td><td>PE4</td><td>3</td><td></td></tr>
   <tr>
   <td>PWRDET</td><td>PC15</td><td>9</td><td></td></tr>
   <tr>
   <td rowspan="2">BLTouch</td>
   <td>SERVOS</td><td>PE5</td><td>4</td><td></td></tr>
   <tr>
   <td>PROBE</td><td>PC13</td><td>7</td><td></td></tr>
   <tr>
   <td rowspan="2">FDCAN</td>
   <td>RX</td><td>PB8</td><td>95</td><td></td></tr>
   <tr>
   <td>TX</td><td>PB9</td><td>96</td><td></td></tr>
   <tr>
   <td rowspan="2">TFT USART1</td>
   <td>RX</td><td>P10</td><td>69</td><td></td></tr>
   <tr>
   <td>TX</td><td>PA9</td><td>68</td><td></td></tr>
   <tr>
   <tr><td rowspan="2">USB-Device</td>
   <td>OTG_FS_DM</td><td>PA11</td><td>70</td><td></td></tr>
   <tr>
   <td>OTG_FS_DP</td><td>PA12</td><td>71</td><td></td></tr>
   <tr>
   <tr><td rowspan="18">LCD-FPC(EXP1 + EXP2)</td>
   <td>5V</td><td>5V</td><td></td><td>EXP1_10</td></tr>
   <tr>
   <td>GND</td><td>GND</td><td></td><td>EXP1_9</td></tr>
   <tr>
   <td>LCD_D7</td><td>PE12</td><td>42</td><td>EXP1_8</td></tr>
   <tr>
   <td>LCD_D6</td><td>PE11</td><td>41</td><td>EXP1_7</td></tr>
   <tr>
   <td>LCD_D5</td><td>PE10</td><td>40</td><td>EXP1_6</td></tr>
   <tr>
   <td>LCD_D4</td><td>PE9</td><td>39</td><td>EXP1_5</td></tr>
   <tr>
   <td>LCD_RS</td><td>PE8</td><td>38</td><td>EXP1_4</td></tr>
   <tr>
   <td>LCD_EN</td><td>PB1</td><td>35</td><td>EXP1_3</td></tr>
   <tr>
   <td>BTN_ENC</td><td>PB0</td><td>34</td><td>EXP1_2</td></tr>
   <tr>
   <td>BEEPER</td><td>PC5</td><td>33</td><td>EXP1_1</td></tr>
   <tr>
   <td>RESET</td><td>NRST</td><td>14</td><td>EXP2_8</td></tr>
   <tr>
   <td>SD_DETECT</td><td>PC4</td><td>32</td><td>EXP2_7</td></tr>
   <tr>
   <td>MOSI</td><td>PA7</td><td>31</td><td>EXP2_6. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td>BTN_EN2</td><td>PB2/td><td>36</td><td>EXP2_5</td></tr>
   <tr>
   <td>SD_SS</td><td>PA4</td><td>28</td><td>EXP2_4</td></tr>
   <tr>
   <td>BTN_EN1</td><td>PE7</td><td>37</td><td>EXP2_3</td></tr>
   <tr>
   <td>SCK</td><td>PA5</td><td>29</td><td>EXP2_2. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td>MISO</td><td>PA6</td><td>30</td><td>EXP2_1. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td rowspan="5">OnboardSD(spi4)</td>
   <td>SD-CS</td><td>PA4</td><td>28</td><td></td></tr>
   <tr>
   <td>SD-DET</td><td>PC4</td><td>32</td><td></td></tr>
   <tr>
   <td>MISO</td><td>PA6</td><td>30</td><td rowspan="3">LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td>
   <tr>
   <td>MOSI</td><td>PA7</td><td>31</td></tr>
   <tr>
   <td>SCK</td><td>PA5</td><td>29</td></tr>
   <tr>
   <td rowspan="9">WIFI(ESP3D/RRF)</td>
   <td>ESP-RST(espResetPin)</td><td>PC14</td><td>8</td><td></td></tr>
   <tr>
   <td>ESP-IO0(espDataReadyPin)</td><td>PB10</td><td>46</td><td></td></tr>
   <tr>
   <td>ESP-IO4(TfrReadyPin)</td><td>PB11</td><td>47</td><td></td></tr>
   <tr>
   <td>ESP-RX(UART7)</td><td>PD9</td><td>56</td><td></td></tr>
   <tr>
   <td>ESP-TX(UART7)</td><td>PD8</td><td>55</td><td></td></tr>
   <tr>
   <td>ESP-CS</td><td>PB12</td><td>51</td><td></td></tr>
   <tr>
   <td>ESP-MOSI-SPI3</td><td>PB15</td><td>54</td><td></td></tr>
   <tr>
   <td>ESP-MISO-SPI3</td><td>PB14</td><td>53</td><td></td></tr>
   <tr>
   <td>ESP-CLK-SPI3</td><td>PB13</td><td>52</td><td></td></tr>
</table>

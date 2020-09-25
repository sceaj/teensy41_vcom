# teensy41_vcom
MCUXpresso (KSDK 2.8.2) Teensy 4.1 project that defines the USB port as a virtual COM port.  This project is based on the KSDK sample evkmimxrt1060_dev_cdc_vcom_bm.

The code creates a USB CDC virtual serial device on the Teensy's USB port and initializes the KSDK Debug Console on LPUART1 (Teensy pins 24[tx] and 25[rx]).

The current version of the code doesn't seem to read from the virtual serial port (this may be because the delay code is interfering with read?), but it is able to write to both the USB and Debug Console successfully. 

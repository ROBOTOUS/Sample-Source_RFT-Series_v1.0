# Getting Started with RFT Series: Sample Code

 

## USB Device Driver Installation

To communicate with RFT sensor with USB interface, you need to configure a PC USB port as a virtual serial port.

Unzip the following file and install the device driver:

>02_USB_Device_Driver\CDM v2.12.24 WHQL Certified(ONLY_WINDOWS)

You can downlaod the latest divice driver from the site below.

```text
http://www.ftdichip.com/Drivers/VCP.htm
```

If you use Linux O/S, please refer to instructions on the same site.

You have to adjust latency of the USB port to reduce the communication latency with the sensor.  Please refer to the following document:

>02_USB_Device_Driver\How to Adjust_Com Port_Latency_ver0.0.pdf

To adjust latency on Linux O/S, please refer to the following file:

>Linux_Serial_Latency_Setting.txt

---

## Sample Program - Windows O/S

You can find execution files in the following directory to communicate with the sensor:

>01_Sample_Source\Windows_OS\bin

To communicate with the F/T sensor with a serial interface (RS232/ RS422/ USB), please use the following file: 

>RFT_IF_UART_SAMPLE_Revx.x.x_r.exe

To communicate with the F/T sensor with CAN interface, please use the following file: 

>RFT_IF_CAN_SAMPLE_Revx.x.x_r.exe (compatible with IXXAT products)

To communicate with the F/T sensor with EtherCAT interface, please use the following files: 

* If you have an EtherCAT adaptor of RFTEC-01, please use the following program:

>RFT_IF_ECAT_EC01_R4_SAMPLE_Revx.x.x_r.exe (SOEM open source)

* If you have an EtherCAT adaptor of RFTEC-02, please use the following program:

>RFT_IF_ECAT_EC02_SAMPLE_Revx.x.x_r.exe (SOEM open source)

* Please make sure you need to install the following file to use SOEM:

>01_Sample_Source\Windows_OS\MISC\WinPcap_for_SOEM

If you fail to execute the files, please install the files in the following directory:

>01_Sample_Source\Windows_OS\MISC\VS2013_Redistribute_Package 

The following sample source was made in Visual Studio 2013:.

>01_Sample_Source\Windows_OS\RFT_IF_CAN_SAMPLE_Rev0.0

>01_Sample_Source\Windows_OS\RFT_IF_UART_SAMPLE_Rev1.2.0

>01_Sample_Source\Windows_OS\RFT_IF_ECAT_EC01_R4_SAMPLE_Rev0.0

To build the sample source for CAN communication, please install the following file:

>01_Sample_Source\Windows_OS\MISC\IXXAT_CAN\vci_v3.5.2\vci_3_5_2_4072.exe 

---

## Additional Sample Source 

To communicate the F/T sensor with a serial interface on Linux O/S, please refer to the following source:

>01_Sample_Source\Linux_OS

To communicate the F/T sensor with EtherCAT interface, please refer to the following source:

**The examples below apply only to the EtherCAT Adaptor of RFTEC-01.**

>01_Sample_Source\SEOM_EtherCAT_Example\SOEM-1.3.1\test\win32\RFTEC01_R4_TEST (for Window O/S)

>01_Sample_Source\SEOM_EtherCAT_Example\SOEM-1.3.1\test\linux\RFTEC01_R4_TEST (for Linux O/S)

**The examples below apply only to the EtherCAT Adaptor of RFTEC-02.**

>01_Sample_Source\SEOM_EtherCAT_Example\SOEM-1.3.1\test\win32\RFTEC02_R0 (for Window O/S)

>01_Sample_Source\SEOM_EtherCAT_Example\SOEM-1.3.1\test\linux\RFTEC02_R0 (for Linux O/S)

To use SOEM (Simple Open EtherCAT Master), please install the following file:

>01_Sample_Source\SEOM_EtherCAT_Example\WinPcapxxx.exe
 
To communicate with the F/T sensor on ROS (Robot Operating System), please refer to the following sample sources of publisher and service node:
		
>01_Sample_Source\ROS\RFT_SENSOR_SERIAL_ver0.0.1_20171218 (for serial communication)

The example below applies only to the EtherCAT Adaptor of RFTEC-01.

>01_Sample_Source\ROS\RFT_SENSOR_ETHERCAT_EC01_R4_20171201 (for EtherCAT communication, SOEM open source)

The example below applies only to the EtherCAT Adaptor of RFTEC-02.

>01_Sample_Source\ROS\ RFT_SENSOR_ETHERCAT_EC02_R0_20180226 (for EtherCAT communication, SOEM open source)

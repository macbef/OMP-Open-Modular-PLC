# OMP-Open-Modular-PLC
**A modular PLC that might some day be open-source**

The professional world is full of PLC manufacturers. They are doing a great job and you can buy almost anything you can think of. 

The DIY world is full of Arduino-like hardware that is ultra flexible and super-easy to program, but you always end up with a lot of PCBs, soldered together like hell and stuffed into cardboard boxes.

But wouldn't it be nice to have something that combines these two worlds? A PLC in a decent housing that is both modular and easy to program?

We took a shot at this and started our own PLC, based on the seasoned STM32F103 controller family and the great stm32duino project.

There are 2 ways to use this PLC:

  * For those who are brave the code of the controller can be modified to match your application
  * A lot easier is using the "stock-firmware".

Here is what it does:

  - auto-detect the connected modules at startup
  - collect data
  - display the current state of all in- and outputs on a tiny OELD display
  - listens to commands on the USB and serial port

The serial commands are easy, jsut like this:

```
"SET 2 3 1"  -> Set Module #2 , Channel #3 to "1"
"GET 3 1"    -> Get the value of channel #1 on module #3
"?"          -> Get all values
```


## Hardware
![demo_02_s](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/bc4a901c-3bf4-41e9-8819-79343546f2d5)
![PLCminiMitDisplay](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/1c653650-4f51-4067-9f07-3e704d1f405f)

![montage_01](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/3e83ede2-5598-4f67-a51a-0e88b228c058)

### Controller

![PLCcontroller_V1_1_iso_s](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/1110a945-aa1d-4932-99c1-25e2b2123d0e)


### Modules

![modules_s](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/19fa7861-c609-492e-9014-1b9ae54fe8c6)

#### Modules built so far (sorry, in German):

![moduleList_1](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/b4714c44-d916-477d-b58f-f123c8ecd978)
![moduleList_2](https://github.com/macbef/OMP-Open-Modular-PLC/assets/26661902/d3d23778-1be9-4b49-8d8a-a6b02faffd4b)



More specs to come....




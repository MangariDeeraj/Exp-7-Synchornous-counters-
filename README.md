# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.


![Screenshot 2023-11-28 103057](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/d050a2bf-5d27-4dae-a564-3fa3623d4a2a)

 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 

Four-bit “Up” Counter

![Screenshot 2023-11-28 103110](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/40f25e3d-a8bd-420a-8f0a-8608316bf2e5)


## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![Screenshot 2023-11-23 220103](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/11fe082e-41c7-4769-bded-e67377e68af1)

 

4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 
/*![Screenshot 2023-11-23 220103](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/a750aab9-7e21-4188-8e63-1e98648aaf63)

Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/






### RTL LOGIC UP COUNTER AND DOWN COUNTER  









### TIMING DIGRAMS FOR COUNTER  
![Screenshot 2023-11-28 103226](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/44eb9c6e-df0f-4978-ac59-afb65c3a5fd5)


![Screenshot 2023-11-23 220314](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/edd9e134-9238-4a7a-b965-a6dbae879b7f)



### TRUTH TABLE 

![WhatsApp Image 2023-11-28 at 10 34 53_23560264](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/853b22d2-109d-40bc-ad3f-148f5205e1eb)
![WhatsApp Image 2023-11-28 at 10 34 53_3f686c61](https://github.com/MangariDeeraj/Exp-7-Synchornous-counters-/assets/149365485/2fc85bbe-40b2-4a23-9621-62d443e78e32)





### RESULTS 

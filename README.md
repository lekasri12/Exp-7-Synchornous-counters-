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



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 

Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: LEKA SRI G
RegisterNumber: 212223100025 
![286807858-4d85de95-545b-4f99-8618-47fa95de3323](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/f168e167-6182-4671-95f4-26d0d5167656)
![286811619-c4f16a82-8f89-4304-9429-ba76f293534f](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/0873df40-c5bc-46ca-8669-5586aa6b271f)

### RTL LOGIC UP COUNTER AND DOWN COUNTER  
![286811767-e703b010-e180-43a4-b8bd-373bed0c43c7](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/c8f314c7-a533-43d5-aa81-5015f7b13e12)
![286811840-25ae01cd-e7c3-423d-8a51-cbe365f859f0](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/a32cbb7c-cbd0-41eb-8d32-921d2c24a288)

### TIMING DIGRAMS FOR COUNTER 
![286811953-bd2a8b29-e52d-4ac8-b3bb-b85fdaeccc8d](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/0d5fa1e2-b2e2-4f50-8b71-be560df84e0b)
![286812000-ee63559a-4125-41ba-9977-cb8afbcc38f3](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/401ba0d9-3739-49d3-bb15-d9bad76be6d0)

### TRUTH TABLE 
![286807905-9f25cb1e-ae2b-4d47-b0d6-27320128726c](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/80102e1f-1de7-4ff2-8c6b-acf19e8d4fe4)
![286811697-b50afb73-d200-466b-ac22-2d844fec24f4](https://github.com/lekasri12/Exp-7-Synchornous-counters-/assets/149037427/4c8491ee-e0d0-4d19-86df-fc19f847ad11)

### RESULTS 
Thus synchornous counters up counter and down counter circuit are studied and the truth table for different logic gates are verified.

# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure:
Step 1: Create module encoder and decoder.
Step 2: Get inputs and outputs for encoders and decoders.
Step 3: Perform "or" operation for encoder and "and" logic for decoders.
Step 4: Perform RTL LOGIC and get waveform.
Step-5: End the module.



### PROGRAM:
Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.
Developed by: DURGA U 
RegisterNumber: 23003210

## CODE:

### ENCODER:
![ENCODER CODE](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/40dd0a58-4381-4d9c-8519-94662823516f)


### DECODER:
![DECODER CODE](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/6448d160-b1d9-4939-a01f-51f62b0d5e90)

## RTL LOGIC:

### ENCODER:
![ENCODER LOGIC](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/88c3f4d0-48dd-47ba-be19-196e821df917)


### DECODER:
![DECODER LOGIC](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/bf9c3c3c-1026-4e42-a4de-7d298551864d)

## TIMING DIGRAMS:

### ENCODER:
![ENCODER TIME](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/7627cf3f-b48d-4849-bc91-75ed4727174d)


### DECODER:
![DECODER TIME](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/30003dcb-5a7a-4117-9f5c-59608b60f7f9)

## TRUTH TABLE:

### ENCODER:
![ENCODER TT](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/056c084f-639b-46d3-8220-ace0fdafd7a7)

### DECODER:
![DECODER T](https://github.com/DurgaUmapathy/Experiment-08-Encoders-and-decoders-/assets/152186191/a7498eea-2c38-4509-b544-06efc610f6ca)


### RESULTS :
Thus the program to desing encoder and decoder is done.

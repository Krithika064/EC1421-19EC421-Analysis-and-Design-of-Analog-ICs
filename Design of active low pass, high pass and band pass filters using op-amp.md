# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
<img width="1280" height="852" alt="image" src="https://github.com/user-attachments/assets/f7cc9065-52da-4797-a1fb-7228327c87bd" />

## HIGH-PASS
<img width="1280" height="844" alt="image" src="https://github.com/user-attachments/assets/d2bc036a-f706-4b71-b502-ffda3726c25a" />

## BAND-PASS
<img width="1280" height="765" alt="image" src="https://github.com/user-attachments/assets/18059f40-904c-408c-be36-201cb4116e0c" />


## MODEL GRAPH:
## LOW_PASS
<img width="1135" height="943" alt="image" src="https://github.com/user-attachments/assets/b59eb0d8-6fac-4956-975e-7a4ad958661e" />

## HIGH-PASS
<img width="1280" height="1136" alt="image" src="https://github.com/user-attachments/assets/a7138a24-7c88-454d-95d6-b8ed22984af8" />

## BAND-PASS
<img width="1249" height="1113" alt="image" src="https://github.com/user-attachments/assets/8e0141d2-05c3-4e1d-8783-b493adae2a40" />


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
<img width="1280" height="1110" alt="image" src="https://github.com/user-attachments/assets/8bbe95cf-ebe4-4743-944e-46cc613af72f" />

## HIGH-PASS
<img width="1249" height="1115" alt="image" src="https://github.com/user-attachments/assets/40f4e56a-d5f2-4a9b-9a46-8c95a526e7d0" />

## BAND-PASS
<img width="1280" height="937" alt="image" src="https://github.com/user-attachments/assets/ace261cd-b28b-44e3-b83b-3de5a323b620" />

## GRAPH:
## LOW_PASS
<img width="1280" height="961" alt="image" src="https://github.com/user-attachments/assets/4db4f26d-b5f5-403e-a21b-7efeeae43f5d" />

## HIGH-PASS
<img width="1280" height="880" alt="image" src="https://github.com/user-attachments/assets/7fcbafa1-d4c7-455a-a424-839bb2d35b10" />

## BAND-PASS
<img width="1280" height="946" alt="image" src="https://github.com/user-attachments/assets/90e2ef4e-2b4e-46a7-8235-73fb72033bcf" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 


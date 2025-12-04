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
![WhatsApp Image 2025-12-04 at 09 33 51_d0dd363f](https://github.com/user-attachments/assets/8adb5dee-c4bf-428e-b695-5b2be72346bd)

## HIGH-PASS
![WhatsApp Image 2025-12-04 at 09 33 50_487261fd](https://github.com/user-attachments/assets/0a21d6c9-44c3-4ff3-8df9-e26b5b987fc4)

## BAND-PASS
![WhatsApp Image 2025-12-04 at 09 33 49_02e27078](https://github.com/user-attachments/assets/5fa0c1e6-16d5-474a-93d8-dcddaf746023)


## MODEL GRAPH:
## LOW_PASS
![WhatsApp Image 2025-12-04 at 09 33 50_e4de7865](https://github.com/user-attachments/assets/e13726c2-bde3-48f3-bc16-5c8311a552d2)

## HIGH-PASS
![WhatsApp Image 2025-12-04 at 09 33 50_d27ebb87](https://github.com/user-attachments/assets/badef700-37c4-471a-9775-949341a26836)

## BAND-PASS
![WhatsApp Image 2025-12-04 at 09 33 48_208fa69e](https://github.com/user-attachments/assets/cf4cd0ac-9a80-485d-a405-58d6cb845e8e)


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
![WhatsApp Image 2025-12-04 at 09 33 50_6652d348](https://github.com/user-attachments/assets/8258b4f8-c0e7-46d0-bea2-afdc2cb02c4d)

## HIGH-PASS
![WhatsApp Image 2025-12-04 at 09 33 49_971ffda5](https://github.com/user-attachments/assets/16b82a44-3b56-41ae-98fd-0f0d8323e86a)

## BAND-PASS
![WhatsApp Image 2025-12-04 at 09 33 48_7dd07df8](https://github.com/user-attachments/assets/537d0512-5c59-46e5-8d1f-e431ef63cbe9)

## CALCULATIONS:
## LOW_PASS
![WhatsApp Image 2025-12-04 at 09 33 48_00efd358](https://github.com/user-attachments/assets/d36b137b-2591-4cdb-8778-a182cb494b7b)

## HIGH-PASS
![WhatsApp Image 2025-12-04 at 09 33 47_ca7c82be](https://github.com/user-attachments/assets/ad51ccb9-a880-4767-9f2e-22585b020348)

## BAND-PASS
![WhatsApp Image 2025-12-04 at 09 33 47_8fd1ff5d](https://github.com/user-attachments/assets/22fd507a-7e09-4731-bddc-f44981aec73b)

## GRAPH:
## LOW_PASS
![WhatsApp Image 2025-12-04 at 09 33 46_66d6563d](https://github.com/user-attachments/assets/bf0f5fae-8385-42c0-93f0-2583e5cf938b)

## HIGH-PASS
![WhatsApp Image 2025-12-04 at 09 33 46_95656397](https://github.com/user-attachments/assets/88c03f80-aff2-4204-81f2-655458440f0b)

## BAND-PASS
![WhatsApp Image 2025-12-04 at 09 33 46_619a07f1](https://github.com/user-attachments/assets/e1170a72-400d-41ae-835c-9d67f4395b6c)

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 


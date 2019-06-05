# BPSK-code-in-MATLAB

It comes under Digital Communication
Binary Phase Shift Keying (BPSK) This is also called as 2-phase PSK or Phase Reversal Keying. ... BPSK is basically a Double Side Band Suppressed Carrier (DSBSC) modulation scheme, for message being the digital information.

					BPSK

clc; 
close all;
clear all;
t=[0:0.01:5*pi];% For setting the sampling interval
A=5;%Amplitude of input signal
wc=2;%For Angular frequency
 
Vi=A.*square(t); % Generating Input Signal
Vc=A.*sin(wc.*t);% Generating Carrier Sine
Vp= Vi.*Vc;% Sine wave multiplied with square wave in order to generate BPSK
 
subplot(3,1,1);% For Plotting Input signal
plot(t,Vi);
xlabel('time')
ylabel('amplitude')
title('Input Signal')
subplot(3,1,2);%For Plotting The Carrier wave
plot(t,Vc);
xlabel('Time')
ylabel('Amplitude')
title('Carrier')
subplot(3,1,3);% For Plotting BPSK (Binary Phase Shift Keying) signal
plot(t,Vp);
xlabel('t')
ylabel('Y')
title('BPSK')





//all the inbuilt command feature are given using //




 



Name:Mayank Chourasia

# Comms-Lab3
Lab 3 repo for communications engineering

### Intro
This repository was formed to contain the deliverables for third lab of EEGR4614 Communications Engineering taught by Professor Allen Morrison.

The purpose of this lab is to demonstrate principles of carrier modulated digital communications by finding the operating frequency of a garage opener unit and demodulate the signal to obtain a binary sequence using a HackRF SDR and GNU Radio Companion software.


### Process
Found on the main page of the repo are screenshots of the various output graphs and GUI sinks as well as the GNU Radio Companion block diagrams and this README.

The block diagram consists of a variable set to 2x10^6 and a QT GUI Range with a start value of 300x10^6 and an end value of 400x10^6. The main block used in this flowgraph is the _Osmocon Source_ block with the sample rate set to 2x10^6 and a frequency of 300x10^6. The output of this Osmocom source block leads to a QT GUI sink, a QU GUI frequency sink, and a complex to mag block followed by a QT GUI time sink. The center frequency of the garage door opener unit can be found with the frequency sink, and the demodulated binary output sequence can be found using the time sink block. the QT GUI sink block includes many more options than just the time or frequency sinks, but the others are recommended for simplicity.


### Conclusion
Throughout this lab, I have gained a much better understanding of demodulation of a signal to binary sequences and how different devices are able to operate around each other which work in the same frequency range without interfering with each other.

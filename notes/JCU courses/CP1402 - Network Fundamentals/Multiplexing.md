---
date: 2024-09-23
location:
  - JCU courses/CP1402 - Network Fundamentalss
hubs:
  - "[[networking]]"
urls:
---

# Definition of multiplexing
+ Multiplexing, or _muxing_, is a way of sending multiple [signals](https://www.techtarget.com/searchnetworking/definition/signal) or streams of information over a communications link at the same time in the form of a single, complex signal. When the signal reaches its destination, a process called _[[Demultiplexing]], or demuxing, recovers the separate signals and outputs them to individual lines.
+ Allow multiple signals to travel simultaneously over one medium
+ To carry multiple signals -> medium's channel is logically separated into multiple smaller channels  (subchannels) (like a tunnel)
+ Multiplexer (mux): device that combines many channel signals

# Types of multiplexing
## WDM (Wavelength division multiplexing)
+ carries mutiple light signals simultaneously -> by dividing light beam -> different wavelengths / colors
## DWDM (Dense wavelength division multiplexing)
+ increases channels more than [[#WDM (Wavelength division multiplexing)]]
## CWDM (Coarse wavelength division multiplexing)
+ lowers cost -> spacing frequency bands wider apart -> cheaper transceiver equipment
(==self explanation==: spaced bands transmission -> less workload on transceiver -> no need for high performing devices to be installed -> save cost)
![[Pasted image 20240918144747.png]]


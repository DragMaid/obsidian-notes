---
date: 2024-09-23
location:
  - JCU courses/CP1402 - Network Fundamentalss
hubs:
  - "[[networking]]"
urls:
---

# Frequency, Bandwidth, Throughput
+ Frequency -> measured in MHz or GHz -> number of times in 1 sec that an electrical signal can change state
+ Bandwidth -> amount of data transmitted in period of time
+ Throughput -> measure how much data actually transmitted in given time period
![[Pasted image 20240918142800.png]]

# Transmission flaws
## Noise
+ Noise undesirable influences degrading or distorting signal (dB - decibels)
+ Two sources of noise:
	1. EMI (electromagnetic interference): by motors, power lines, TV, ...
	2. Cross-talk: wire infringes (break a law or rule) on adjacent wire signal:
		+ Alien cross-talk -> between two cables
		+ Near end cross-talk (NEXT) occurs near source
		+ Far end cross-talk (FEXT) occurs near far end

## Technical terms
+ Attenuation: loss of signal strength as it travels away from source -> can be boosted via a [[repeater]] (like red-stone signal strength)
+ Latency: delay between transmission and receipt (amount of time that you are late for your date)
+ RTT (round trip time): time for packet to go from sender to receiver and back (just like the chu kì in physics)
+ Packets arrive varying delay -> out of order (called jitter or PDV - packet delay variation)

# Duplex, Half-Duplex and Simplex
## Full duplex
+ Signals travel both directions over a medium simultaneously (two lanes road)

## Half duplex
+ Signals travel both directions over a medium simultaneously but only in one direction at a time(one lane road)

## Simplex
+ Signals travel in only one direction (also called one-way or unidirectional communication)

## [[Multiplexing]]

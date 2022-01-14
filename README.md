# RDAHAM
Ham Radio Station based around the RDA1846s (maybe more)
----

## TBD 
This is just a Thought-project at this stage. Will update later if i recieve hardware and revise it following.

## GOALS

1. Dual-Band UHF/VHF Ham Radio.
3. Use dual analog & digital meters/interface to allow robust operation. (If possible a LCD for Microcontroller control and waterfall[if possible]) 
4. Expose the GPIO/i2c interface to a SOC to operate the RDA1846S.
6. Use rotary nobs and multi/single throw toggles(with software sliders for disabling them if driven by TS-LCD) for tactile control. keypad for DTMF (and touch sensitive LCD if possible)
7. Slave as much as possible to the RDA1846S, using SOC in addinum where possible(replace these functions in software optionally via menu/switches?)
8. Analog (Direct) & Digitial modes via Software(Seperate SOC for this?).
9. Antenna amp external to RDA1846S[I am uncertain if the 1846S has a pre-amp atm, proceeding assuming it exists.]. offering 4-stages: ULP(2w nom, on-chip), LP(5w nom, on-chip), normal(? - ???w, rotary nob set variable amp), line-driven (no-preamp)
10. Antenna RX pre-amp. 
10. Trigger VOX on toggle, rather than microcontroller driven to prevent accidental activation. 
11. Add software SQ additionally to hardware SQ, with toggle to disable hardware SQ and software SQ on rotary (with LCD menu as well if LCD is present)
12. Toggles to disable AFC/AGC
13. RSSI with both digital numerical counter and analog meter.
14. CTCSS/CDCSS via rotary (with locked range)
15. DCS bit/code displayed via small lcd.

## Like-to-do

1. Multi-antenna (RX/TX)
2. Duplex capable (optionally dual 1846s or SDR for this mode)
3. LCD for fine control and additional options.
4. Waterfall? (IDK if the 1846s would even be capable of producing the data for this. need more research)
5. include HF tranciever for HF bands with input for CW lever.
6. include frequency shifter for 23cm band.
7. include SHF tranciever for experimental 3-5ghz bands.
8. include SDR to exclusively drive waterfall seperate to transciever (hackRF/RSP1S seems possible, HackRF could do HF/SHF Trancieving but poor interfacing and cost might prohibit. might be better to use RTL and find a way to use the tranciever to do tuning)

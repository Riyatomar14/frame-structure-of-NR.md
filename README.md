# frame-structure-of-NR.md

![Screenshot 2023-11-08 160334](https://github.com/Riyatomar14/frame-structure-of-NR.md/assets/143107173/b7bcc1d9-778f-47ed-adf3-8811339a3ed8)

1.**Radio frames**-radio frames used in transferring the data (uplink/downlink) in the air. Its duration is 10 milliseconds.

2. **sub-frames**-one radio frames of 10ms is divided 10 sub-frames which is of length 1 millisecond.Subframes inside a radio frame are serialized as SF0, SF1, SF2, SF3, …., and SF9.

3. **Resource grid**- A subframe is made up of a Resource Grid which is a (m x n) matrix of Resource Elements where ‘m’ defines the number of Sub-carriers and ‘n’ defines the number of OFDM(orthogonal frequency division mutiplexer) Symbols.

4.**SCS(SubCarrier Spacing)**-subframe is further divided into slots.these slots is varies in NR, depending upon SCS.Slot length gets shorter as Subcarrier 

Spacing gets wider.

note point-Formula to calculate, SCS = 15 x 2μ kHz(where μ = 0, 1, 2, 3, 4)

5.**Resource block**-resource block,in which a slot is divided into 12 sub carrier.

6.**Slot**-It is divided into into 2 parts on the basis of number of OFDM. The number of OFDM Symbols varies with slot configuration, and the type of Cyclic

Prefix used.

 a> Slot Configuration 0-The number of symbols in a slot is always 14 for Normal Cyclic Prefix and 12 for Extended Cyclic Prefix. 
 
 b> Slot Configuration 1 -– In this configuration, the number of symbols in a slot is always 7 for Normal Cyclic Prefix and 6 for Extended Cyclic Prefix.
 
 This is the old Slot configuration mechanism used in the 4G System for resource allocation.

 7.

 

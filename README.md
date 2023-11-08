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

 7.**OFDM(Orthogonal Frequency Division Multiplexing)**-It is a modulation technique in which wide frequency band is split into many, small frequency called
 
 subcarriers, transmit in such a way that they overlap each other but do not influence other subcarriers. these carrier wave are orthogonal which means that 
  
 one is at the peaak and other is at the null .

 8.**QAM(Quadrature Amplitude Modulation) and FDM(Frequency Division Modulation)**-technique to increase the channel efficiency and reduce bandwidth 
 
 consumption, ultimately producing a high data rate .

 9.**ISI(Inter Symbol Interference)**-if mutiple signal is comming destination so due to which signals get distorted by fading and the doppler effect.

  If one symbol gets delayed a bit, then it coincides with the next symbol and causes interference.

 10.**time gap**-To overcome this problem, a time gap is introduced between every 2 symbols.But leaving the space empty like turning off the transmission, 
 
 would cause problems for the amplifier. So, to encounter this, a CP(Cyclic Prefix) is introduced in the space.

 11.**Cyclic Prefix**-The Cyclic Prefix in OFDM refers to copying the end part of the signal and adding it at the beginning of it.

 Cyclic Prefix is of 2 types –

  **Normal CP** – In Normal CP, the slot is divided into 14/7 symbols based on slot configuration. The normal CP length is designed to support propagation 
 
 conditions with a delay spread up to 4.7 μs.

  **Extended CP** – The slot is divided into 12/6 OFDM symbols based on slot configuration in the case of extended CP. This is intended to support 

    deployments where the delay spread is up to 16.7 μs. This is only supported for the μ value 2 i.e. 60KHz SCS.

 12.
 

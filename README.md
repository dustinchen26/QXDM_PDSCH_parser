# QXDM NR5G PDSCH Parser - Slot Error Rate
● ssb_basic : https://dustinchen26.github.io/QXDM_PDSCH_parser

## Example
● input
```
17:29:19.449705          LOG                      [0xB887]                 NR5G MAC PDSCH Status                                       1                        Length:   88
17:29:19.449705	[0xB887]	NR5G MAC PDSCH Status
MacVersion {
   Major.Minor = 2
   5
}
Version 131077 {
   Log Fields Change {
   }
   Log Fields Change BMask = 0x0
   Sub ID = 0
   Num Records = 2
   Records[0] {
      System Time {
         Slot = 16
         Numerology =    30kHz
         Frame = 631
      }
      Num PDSCH Status = 1
      PDSCH Status Info[0] {
         Carrier ID = 0
         Tech Id = 1
         Opcode = 0
         Conn ID = 0
         Bandwidth = 12
         Band Type = 0
         Variant Id = 0
         Physical cell ID = 186
         EARFCN =   644736
         TB Index = 0
         TB Size =     1281
         SCS MU = 1
         MCS = 18
         Num Rbs =    4
         RV = 0
         HARQ Or MBSFN Area Id = 5
         RNTI Type = 0
         K1 Or PMCH ID = 3
         TCI = 0
         Num Layers = 4
         Iteration Index = 0
         CRC State =     PASS
         CRC Status = PASS
         New Tx Flag = 1
         NDI = 0
         Discard Mode = 0
         Bypass Decode = 0
         Bypass HARQ = 0
         Num ReTx = 0
         HD Onload Timeout = 0
         HARQ Onload Timeout = 0
         HD Offload Timeout = 0
         HARQ Offload Timeout = 0
         Did Recomb = 0
         Is IOVec Valid = true
         Mod Type =   64_QAM
         High Clock Mode = 0
         Num RX = 4x4_MIMO
         RX Antenna Mapping 0 = 0
         RX Antenna Mapping 1 = 0
         RX Antenna Mapping 2 = 0
         RX Antenna Mapping 3 = 0
      }
```
● output
```
總筆數：1，CRC FAIL 筆數：0，❗ Error Rate（總）：0.00%
Slot 16 | Error Rate = 0.00% (0/1)
Frame	Slot	CRC Status	CRC State	HARQ Id	K1	MCS	Num Rbs	TB Size	NDI	RV	Num Layers	Mod Type
631	16	PASS	PASS	5	3	18	4	1281	0	0	4	64_QAM
```

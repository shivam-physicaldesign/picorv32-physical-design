# picorv32 RISC-V Processor Physical Design — sky130A PDK

Complete RTL-to-GDSII physical design of the picorv32 RISC-V processor using OpenLane on Google/SkyWater sky130A 130nm PDK.

## Results

| Metric | Value |
|--------|-------|
| Clock Frequency | 200 MHz |
| Clock Period | 5.0 ns |
| Critical Path | 4.79 ns |
| WNS | 0.0 ns |
| TNS | 0.0 ns |
| Total Cells | 84,688 |
| Die Area | 0.81 mm² |
| Wire Length | 687,596 µm |
| DRC Violations | 0 |
| LVS Errors | 0 |

## Frequency Sweep Summary

| Period | Frequency | Result |
|--------|-----------|--------|
| 15 ns | 66 MHz | ✅ Clean |
| 10 ns | 100 MHz | ✅ Clean |
| 6 ns | 166 MHz | ✅ Clean |
| 5 ns | 200 MHz | ✅ Clean — Maximum |
| 4.5 ns | 222 MHz | ❌ Setup violations |

## Flow
RTL → Synthesis (Yosys) → Floorplan → Placement → CTS → Routing → DRC/LVS → GDSII

## Tools
- OpenLane v1.0.2
- sky130A PDK (Google/SkyWater 130nm)
- OpenROAD, TritonCTS, TritonRoute, Magic, Netgen

## About picorv32
picorv32 is a production-quality RISC-V RV32IMC processor core by Clifford Wolf, widely used in open-source chip design and real tapeouts.

## Author
Shivam Kumar Maurya — B.Tech ECE, VNRVJIET (2022–2026)

## Layout

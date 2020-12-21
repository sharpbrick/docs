# TechnicDistanceSensor

Ultrasound based distance sensor (originally part of Spike Prime and Mindstorms)

**Type**: External Sensor

**Status**: Well Defined (Exploration for extension interface)

## Modes

### Mode 0 - Long Range Distance (DISTL)

Complete range from 0 to 250cm. Everything above is set to 0 and not reporting changes.

**Direction**: Input

**DataType**: Int16 reprecenting cm (positive)

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).
- ⚠ Sub integer scaling (change of data type needed)


### Mode 1 - Short Range Distance (DISTS)

Mode specialized on short range distance. Everything above 32cm is set to 0 and not reporting changes.

**Direction**: Input

**DataType**: Int16 reprecenting cm (positive)

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).
- ⚠ Sub integer scaling (change of data type needed)

### Mode 2 - Single Value reported Distance (SINGL)

Reporting a single reported value when subscribed (no updates).

**Direction**: Input

**DataType**: Int16 reprecenting cm (positive)

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).
- ⚠ Sub integer scaling (change of data type needed)

### Mode 3 - LISTN

TODO: Boolean flag (most likely for something like listen)

**Direction**: Input

**DataType**: SByte reprecenting a boolean value 0 or 1

### Mode 4 - Raw Ultrasound Sensor Output (TRAW)

Reporting (most likely) the cycle time between ultrasound emission and receiving in uS.

**Direction**: Input

**DataType**: Int32 representing uS

### Mode 5 - Eye Lights (LIGHT)

Reporting a single reported value when subscribed (no updates).

**Direction**: Output

**DataType**: 4 SByte with brightness values of 0-100. Byte order is left-top, right-top, left-bottom, right-bottom (seen from the fron with Lego Logo readable)

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).
- ⚠ Sub integer scaling (change of data type needed)

### Mode 6 - Ping

TODO Description

**Direction**: Input | Output

**DataType**: TODO

**Notes**
- TODO

### Mode 7 - ADRAW

TODO: Unclear Definition (most likely related to extension interface)

### Mode 8 - CALIB

TODO: Unclear Definition

## Known Related Commands

- WriteDirectModeDataMessage for Light

## Supplementary Definitions

### Extension interface on the adapter

The sensor has an electric interface allowing additional signals to be connected.

## Open Questions

- Why the SINGL query option? That is part of the protocol itself to query for updates or single value.
- Defintion for the extension interface.

## Port and Port Mode Information

### Software 1.0.0.0 / Hardware 1.0.0.0

Binary Export

````
0B-00-43-00-01-03-09-9F-00-60-00
05-00-43-00-02
11-00-44-00-00-00-44-49-53-54-4C-00-00-00-00-00-00
0E-00-44-00-00-01-00-00-00-00-00-40-1C-45
0E-00-44-00-00-02-00-00-00-00-00-00-C8-42
0E-00-44-00-00-03-00-00-00-00-00-00-7A-43
0A-00-44-00-00-04-43-4D-00-00
08-00-44-00-00-05-91-00
0A-00-44-00-00-80-01-01-05-01
11-00-44-00-01-00-44-49-53-54-53-00-00-00-00-00-00
0E-00-44-00-01-01-00-00-00-00-00-00-A0-43
0E-00-44-00-01-02-00-00-00-00-00-00-C8-42
0E-00-44-00-01-03-00-00-00-00-00-00-00-42
0A-00-44-00-01-04-43-4D-00-00
08-00-44-00-01-05-F1-00
0A-00-44-00-01-80-01-01-04-01
11-00-44-00-02-00-53-49-4E-47-4C-00-00-00-00-00-00
0E-00-44-00-02-01-00-00-00-00-00-40-1C-45
0E-00-44-00-02-02-00-00-00-00-00-00-C8-42
0E-00-44-00-02-03-00-00-00-00-00-00-7A-43
0A-00-44-00-02-04-43-4D-00-00
08-00-44-00-02-05-90-00
0A-00-44-00-02-80-01-01-05-01
11-00-44-00-03-00-4C-49-53-54-4E-00-00-00-00-00-00
0E-00-44-00-03-01-00-00-00-00-00-00-80-3F
0E-00-44-00-03-02-00-00-00-00-00-00-C8-42
0E-00-44-00-03-03-00-00-00-00-00-00-80-3F
0A-00-44-00-03-04-53-54-00-00
08-00-44-00-03-05-10-00
0A-00-44-00-03-80-01-00-01-00
11-00-44-00-04-00-54-52-41-57-00-00-00-00-00-00-00
0E-00-44-00-04-01-00-00-00-00-00-C4-63-46
0E-00-44-00-04-02-00-00-00-00-00-00-C8-42
0E-00-44-00-04-03-00-00-00-00-00-C4-63-46
0A-00-44-00-04-04-75-53-00-00
08-00-44-00-04-05-90-00
0A-00-44-00-04-80-01-02-05-00
11-00-44-00-05-00-4C-49-47-48-54-00-00-00-00-00-00
0E-00-44-00-05-01-00-00-00-00-00-00-C8-42
0E-00-44-00-05-02-00-00-00-00-00-00-C8-42
0E-00-44-00-05-03-00-00-00-00-00-00-C8-42
0A-00-44-00-05-04-50-43-54-00
08-00-44-00-05-05-00-10
0A-00-44-00-05-80-04-00-03-00
11-00-44-00-06-00-50-49-4E-47-00-00-00-00-00-00-00
0E-00-44-00-06-01-00-00-00-00-00-00-80-3F
0E-00-44-00-06-02-00-00-00-00-00-00-C8-42
0E-00-44-00-06-03-00-00-00-00-00-00-80-3F
0A-00-44-00-06-04-50-43-54-00
08-00-44-00-06-05-00-90
0A-00-44-00-06-80-01-00-01-00
11-00-44-00-07-00-41-44-52-41-57-00-00-00-00-00-00
0E-00-44-00-07-01-00-00-00-00-00-00-80-44
0E-00-44-00-07-02-00-00-00-00-00-00-C8-42
0E-00-44-00-07-03-00-00-00-00-00-00-80-44
0A-00-44-00-07-04-50-43-54-00
08-00-44-00-07-05-90-00
0A-00-44-00-07-80-01-01-04-00
11-00-44-00-08-00-43-41-4C-49-42-00-00-00-00-00-00
0E-00-44-00-08-01-00-00-00-00-00-00-7F-43
0E-00-44-00-08-02-00-00-00-00-00-00-C8-42
0E-00-44-00-08-03-00-00-00-00-00-00-7F-43
0A-00-44-00-08-04-50-43-54-00
08-00-44-00-08-05-00-00
0A-00-44-00-08-80-07-00-03-00
````

Human Readable Interpretation

````
  - Port: 0x00 / 0
    - IOTypeId: TechnicDistanceSensor / 0x003E / 62
      Revision: SW: 1.0.0.0, HW: 1.0.0.0
      Capabilities: Output Input
      ModeCombinations: []
    - Mode 0: Name: DISTL, Symbol: CM, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 5, Decimals: 1
        Input Mapping: SupportsNull Absolute
        Raw Min:       0, Max:    2500
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     250 (scaling)
    - Mode 1: Name: DISTS, Symbol: CM, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 4, Decimals: 1
        Input Mapping: SupportsNull SupportFunctionalMapping20 Absolute
        Raw Min:       0, Max:     320
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      32 (scaling)
    - Mode 2: Name: SINGL, Symbol: CM, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 5, Decimals: 1
        Input Mapping: SupportsNull Absolute
        Raw Min:       0, Max:    2500
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     250 (scaling)
    - Mode 3: Name: LISTN, Symbol: ST, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 1, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:       1
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:       1 (pass-through)
    - Mode 4: Name: TRAW, Symbol: uS, Capability: Input
      - DataSet: 1x Int32, TotalFigures: 5, Decimals: 0
        Input Mapping: SupportsNull Absolute
        Raw Min:       0, Max:   14577
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:   14577 (pass-through)
    - Mode 5: Name: LIGHT, Symbol: PCT, Capability: Output
      - DataSet: 4x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 6: Name: PING, Symbol: PCT, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 1, Decimals: 0
        Output Mapping: SupportsNull Absolute
        Raw Min:       0, Max:       1
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:       1 (pass-through)
    - Mode 7: Name: ADRAW, Symbol: PCT, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: SupportsNull Absolute
        Raw Min:       0, Max:    1024
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    1024 (pass-through)
    - Mode 8: Name: CALIB, Symbol: PCT, Capability:
      - DataSet: 7x SByte, TotalFigures: 3, Decimals: 0
        Raw Min:       0, Max:     255
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     255 (pass-through)
````
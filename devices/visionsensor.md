# VisionSensor

Color & distance sensor which is sold as it is own part.

**Type**: External Sensor

**Status**: Pending Issues

## Modes

### Mode 0 - Color

Detecting distinct LEGO Colors

**Direction**: Input

**DataType**: SByte expressing the discrete value of the color. See table.

**Notes**
- -1 if no color could be identified.

### Mode 1 - Proximity

Reports the distance to the closes object in an abstract way, 0 for close and 10 for far away.

TODO: Further testing required for the range

**Direction**: Input

**DataType**: SByte (0-10)

### Mode 2 - Count

Unclear, jumps by 5 it seems when observed

**Direction**: Input

**DataType**: Int32 (0-100)

### Mode 3 - Reflection

Light reflected from the surface on which the sensor is applied to.

**Direction**: Input

**DataType**: SByte (0-100)

### Mode 4 - Ambient Light

The Ambient Light received by the sensor

**Direction**: Input

**DataType**: SByte (0-100)

### Mode 5 - Color

TODO: Unclear Definition

**Direction**: Output

**DataType**: SByte

### Mode 6 - RGB Sensor

Color in RGB encoding (however, value range in 0-1023)

**Direction**: Input

**DataType**: 3x Int16 (r, g, b each in 0-1023)

### Mode 7 - IRTx

TODO: Unclear Definition

**Direction**: Output

**DataType**: Int16

### Mode 8 - SPEC1

TODO: Unclear Definition

### Mode 9 - Debug

TODO: Unclear Definition

**Direction**: Input

**DataType**: 2x Int16

### Mode 10 - Debug

TODO: Unclear Definition

**Direction**: Input

**DataType**: 8x Int16

## Supplementary Definitions

### Color

| Idx | Color |
| --- | --- |
| -1 | n/a |
| 0 | Black |
| 3 | Blue |
| 4 | Teal |
| 5 | Green |
| 7 | Yellow |
| 9 | Red |
| 10 | White |

## Open Questions

- Check color table if it matches the copied one from the TechnicColorSensor
- Check what DEBUG and CALIB output
- More and preciser testing for Proximity is required

## Port and Port Mode Information

### Software 1.0.0.0 / Hardware 1.0.0.0

Binary Export

````
0B-00-43-01-01-07-0B-5F-06-A0-00
07-00-43-01-02-4F-00
12-00-44-01-00-00-43-4F-4C-4F-52-00-00-00-00-00-00-00
0E-00-44-01-00-01-00-00-00-00-00-00-20-41
0E-00-44-01-00-02-00-00-00-00-00-00-C8-42
0E-00-44-01-00-03-00-00-00-00-00-00-20-41
0B-00-44-01-00-04-49-44-58-00-00
08-00-44-01-00-05-C4-00
0A-00-44-01-00-80-01-00-03-00
12-00-44-01-01-00-50-52-4F-58-00-00-00-00-00-00-00-00
0E-00-44-01-01-01-00-00-00-00-00-00-20-41
0E-00-44-01-01-02-00-00-00-00-00-00-C8-42
0E-00-44-01-01-03-00-00-00-00-00-00-20-41
0B-00-44-01-01-04-44-49-53-00-00
08-00-44-01-01-05-50-00
0A-00-44-01-01-80-01-00-03-00
12-00-44-01-02-00-43-4F-55-4E-54-00-00-00-00-00-00-00
0E-00-44-01-02-01-00-00-00-00-00-00-C8-42
0E-00-44-01-02-02-00-00-00-00-00-00-C8-42
0E-00-44-01-02-03-00-00-00-00-00-00-C8-42
0B-00-44-01-02-04-43-4E-54-00-00
08-00-44-01-02-05-08-00
0A-00-44-01-02-80-01-02-04-00
12-00-44-01-03-00-52-45-46-4C-54-00-00-00-00-00-00-00
0E-00-44-01-03-01-00-00-00-00-00-00-C8-42
0E-00-44-01-03-02-00-00-00-00-00-00-C8-42
0E-00-44-01-03-03-00-00-00-00-00-00-C8-42
0B-00-44-01-03-04-50-43-54-00-00
08-00-44-01-03-05-10-00
0A-00-44-01-03-80-01-00-03-00
12-00-44-01-04-00-41-4D-42-49-00-00-00-00-00-00-00-00
0E-00-44-01-04-01-00-00-00-00-00-00-C8-42
0E-00-44-01-04-02-00-00-00-00-00-00-C8-42
0E-00-44-01-04-03-00-00-00-00-00-00-C8-42
0B-00-44-01-04-04-50-43-54-00-00
08-00-44-01-04-05-10-00
0A-00-44-01-04-80-01-00-03-00
12-00-44-01-05-00-43-4F-4C-20-4F-00-00-00-00-00-00-00
0E-00-44-01-05-01-00-00-00-00-00-00-20-41
0E-00-44-01-05-02-00-00-00-00-00-00-C8-42
0E-00-44-01-05-03-00-00-00-00-00-00-20-41
0B-00-44-01-05-04-49-44-58-00-00
08-00-44-01-05-05-00-04
0A-00-44-01-05-80-01-00-03-00
12-00-44-01-06-00-52-47-42-20-49-00-00-00-00-00-00-00
0E-00-44-01-06-01-00-00-00-00-00-C0-7F-44
0E-00-44-01-06-02-00-00-00-00-00-00-C8-42
0E-00-44-01-06-03-00-00-00-00-00-C0-7F-44
0B-00-44-01-06-04-52-41-57-00-00
08-00-44-01-06-05-10-00
0A-00-44-01-06-80-03-01-05-00
12-00-44-01-07-00-49-52-20-54-78-00-00-00-00-00-00-00
0E-00-44-01-07-01-00-00-00-00-00-FF-7F-47
0E-00-44-01-07-02-00-00-00-00-00-00-C8-42
0E-00-44-01-07-03-00-00-00-00-00-FF-7F-47
0B-00-44-01-07-04-4E-2F-41-00-00
08-00-44-01-07-05-00-04
0A-00-44-01-07-80-01-01-05-00
12-00-44-01-08-00-53-50-45-43-20-31-00-00-00-00-00-00
0E-00-44-01-08-01-00-00-00-00-00-00-7F-43
0E-00-44-01-08-02-00-00-00-00-00-00-C8-42
0E-00-44-01-08-03-00-00-00-00-00-00-7F-43
0B-00-44-01-08-04-4E-2F-41-00-00
08-00-44-01-08-05-00-00
0A-00-44-01-08-80-04-00-03-00
12-00-44-01-09-00-44-45-42-55-47-00-00-00-00-00-00-00
0E-00-44-01-09-01-00-00-00-00-00-C0-7F-44
0E-00-44-01-09-02-00-00-00-00-00-00-C8-42
0E-00-44-01-09-03-00-00-00-00-00-00-20-41
0B-00-44-01-09-04-4E-2F-41-00-00
08-00-44-01-09-05-10-00
0A-00-44-01-09-80-02-01-05-00
12-00-44-01-0A-00-43-41-4C-49-42-00-00-00-00-00-00-00
0E-00-44-01-0A-01-00-00-00-00-00-FF-7F-47
0E-00-44-01-0A-02-00-00-00-00-00-00-C8-42
0E-00-44-01-0A-03-00-00-00-00-00-FF-7F-47
0B-00-44-01-0A-04-4E-2F-41-00-00
08-00-44-01-0A-05-10-00
0A-00-44-01-0A-80-08-01-05-00
````

Human Readable Interpretation

````
  - Port: 0x01 / 1
    - IOTypeId: VisionSensor / 0x0025 / 37
      Revision: SW: 1.0.0.0, HW: 1.0.0.0
      Capabilities: Output Input LogicalCombinable  
      ModeCombinations: [0000000001001111]
    - Mode 0: Name: COLOR, Symbol: IDX, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: SupportsNull SupportFunctionalMapping20 Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 1: Name: PROX, Symbol: DIS, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: SupportFunctionalMapping20 Absolute
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 2: Name: COUNT, Symbol: CNT, Capability: Input
      - DataSet: 1x Int32, TotalFigures: 4, Decimals: 0
        Input Mapping: Relative
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 3: Name: REFLT, Symbol: PCT, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 4: Name: AMBI, Symbol: PCT, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 5: Name: COL O, Symbol: IDX, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 6: Name: RGB I, Symbol: RAW, Capability: Input
      - DataSet: 3x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    1023
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    1023 (pass-through)
    - Mode 7: Name: IR Tx, Symbol: N/A, Capability: Output
      - DataSet: 1x Int16, TotalFigures: 5, Decimals: 0
        Output Mapping: Discrete
        Raw Min:       0, Max:   65535
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:   65535 (pass-through)
    - Mode 8: Name: SPEC 1, Symbol: N/A, Capability:
      - DataSet: 4x SByte, TotalFigures: 3, Decimals: 0
        Raw Min:       0, Max:     255
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     255 (pass-through)
    - Mode 9: Name: DEBUG, Symbol: N/A, Capability: Input
      - DataSet: 2x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    1023
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (scaling)
    - Mode 10: Name: CALIB, Symbol: N/A, Capability: Input
      - DataSet: 8x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:   65535
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:   65535 (pass-through)
````
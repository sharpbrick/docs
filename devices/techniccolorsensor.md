# TechnicColorSensor

Color sensor which is part of the Lego Mindstorms (51515) set.

**Type**: External Sensor

**Status**: Pending Issues

## Modes

### Mode 0 - Color

Detecting distinct LEGO Colors

**Direction**: Input

**DataType**: sbyte expressing the discrete value of the color. See table.

**Notes**
- -1 if no color could be identified.

### Mode 1 - Reflection

Light reflected from the surface on which the sensor is applied to.

**Direction**: Input

**DataType**: sbyte (0-100)

### Mode 2 - Ambient Light

The Ambient Light received by the sensor

**Direction**: Input

**DataType**: sbyte (0-100)

**Notes**
- A notification deltaInterval of 1 is recommendable.

### Mode 3 - Sector Lights (LIGHT)

Three LEDS around the sensor illumating the scanned area. By default all one with full brightness.

**Direction**: Output

**DataType**: 3x sbyte with value ranges 0-100 defining brightness.

**Notes**
- Only works if after the WriteDirectPortModeData a PortInputFormatSetupSingleMessage is sent to the mode (as with the RgbLight)

### Mode 4 - RawReflection

Raw Data (most likely for Mode 1)

### Mode 5 - RGB Sensor

Color in RGB encoding (however, value range in 0-1024)

**Direction**: Input

**DataType**: 4x Int16 (r, g, b each in 0-1024) ... fourth value unknown.

### Mode 6 - HSV Sensor

Color in HSV encoding

**Direction**: Input

**DataType**: 3x Int16 (hue, saturation, value)

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

A shade of purple is missing, most likely in 1 or 2 (reference Mindstorm App Color selector)

## Open Questions

- Complete Color Table Definition.
- Why the port needs to be formated after the lights are instructed.

## Port and Port Mode Information

### Software 1.0.0.0 / Hardware 1.0.0.0

Binary Export

````
0B-00-43-01-01-07-0A-F7-01-08-00
07-00-43-01-02-63-00
11-00-44-01-00-00-43-4F-4C-4F-52-00-00-00-00-00-00
0E-00-44-01-00-01-00-00-00-00-00-00-20-41
0E-00-44-01-00-02-00-00-00-00-00-00-C8-42
0E-00-44-01-00-03-00-00-00-00-00-00-20-41
0A-00-44-01-00-04-49-44-58-00
08-00-44-01-00-05-E4-00
0A-00-44-01-00-80-01-00-02-00
11-00-44-01-01-00-52-45-46-4C-54-00-00-00-00-00-00
0E-00-44-01-01-01-00-00-00-00-00-00-C8-42
0E-00-44-01-01-02-00-00-00-00-00-00-C8-42
0E-00-44-01-01-03-00-00-00-00-00-00-C8-42
0A-00-44-01-01-04-50-43-54-00
08-00-44-01-01-05-30-00
0A-00-44-01-01-80-01-00-03-00
11-00-44-01-02-00-41-4D-42-49-00-00-00-00-00-00-00
0E-00-44-01-02-01-00-00-00-00-00-00-C8-42
0E-00-44-01-02-02-00-00-00-00-00-00-C8-42
0E-00-44-01-02-03-00-00-00-00-00-00-C8-42
0A-00-44-01-02-04-50-43-54-00
08-00-44-01-02-05-30-00
0A-00-44-01-02-80-01-00-03-00
11-00-44-01-03-00-4C-49-47-48-54-00-00-00-00-00-00
0E-00-44-01-03-01-00-00-00-00-00-00-C8-42
0E-00-44-01-03-02-00-00-00-00-00-00-C8-42
0E-00-44-01-03-03-00-00-00-00-00-00-C8-42
0A-00-44-01-03-04-50-43-54-00
08-00-44-01-03-05-00-10
0A-00-44-01-03-80-03-00-03-00
11-00-44-01-04-00-52-52-45-46-4C-00-00-00-00-00-00
0E-00-44-01-04-01-00-00-00-00-00-00-80-44
0E-00-44-01-04-02-00-00-00-00-00-00-C8-42
0E-00-44-01-04-03-00-00-00-00-00-00-80-44
0A-00-44-01-04-04-52-41-57-00
08-00-44-01-04-05-10-00
0A-00-44-01-04-80-02-01-04-00
11-00-44-01-05-00-52-47-42-20-49-00-00-00-00-00-00
0E-00-44-01-05-01-00-00-00-00-00-00-80-44
0E-00-44-01-05-02-00-00-00-00-00-00-C8-42
0E-00-44-01-05-03-00-00-00-00-00-00-80-44
0A-00-44-01-05-04-52-41-57-00
08-00-44-01-05-05-10-00
0A-00-44-01-05-80-04-01-04-00
11-00-44-01-06-00-48-53-56-00-00-00-00-00-00-00-00
0E-00-44-01-06-01-00-00-00-00-00-00-B4-43
0E-00-44-01-06-02-00-00-00-00-00-00-C8-42
0E-00-44-01-06-03-00-00-00-00-00-00-B4-43
0A-00-44-01-06-04-52-41-57-00
08-00-44-01-06-05-10-00
0A-00-44-01-06-80-03-01-04-00
11-00-44-01-07-00-53-48-53-56-00-00-00-00-00-00-00
0E-00-44-01-07-01-00-00-00-00-00-00-B4-43
0E-00-44-01-07-02-00-00-00-00-00-00-C8-42
0E-00-44-01-07-03-00-00-00-00-00-00-B4-43
0A-00-44-01-07-04-52-41-57-00
08-00-44-01-07-05-10-00
0A-00-44-01-07-80-04-01-04-00
11-00-44-01-08-00-44-45-42-55-47-00-00-00-00-00-00
0E-00-44-01-08-01-00-00-00-00-00-FF-7F-47
0E-00-44-01-08-02-00-00-00-00-00-00-C8-42
0E-00-44-01-08-03-00-00-00-00-00-FF-7F-47
0A-00-44-01-08-04-52-41-57-00
08-00-44-01-08-05-10-00
0A-00-44-01-08-80-04-01-04-00
11-00-44-01-09-00-43-41-4C-49-42-00-00-00-00-00-00
0E-00-44-01-09-01-00-00-00-00-00-FF-7F-47
0E-00-44-01-09-02-00-00-00-00-00-00-C8-42
0E-00-44-01-09-03-00-00-00-00-00-FF-7F-47
0A-00-44-01-09-04-00-00-00-00
08-00-44-01-09-05-00-00
0A-00-44-01-09-80-07-01-05-00
````

Human Readable Interpretation

````
  - Port: 0x01 / 1
    - IOTypeId: TechnicColorSensor / 0x003D / 61
      Revision: SW: 1.0.0.0, HW: 1.0.0.0
      Capabilities: Output Input LogicalCombinable
      ModeCombinations: [0000000001100011]
    - Mode 0: Name: COLOR, Symbol: IDX, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 2, Decimals: 0
        Input Mapping: SupportsNull SupportFunctionalMapping20 Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 1: Name: REFLT, Symbol: PCT, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 2: Name: AMBI, Symbol: PCT, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 3: Name: LIGHT, Symbol: PCT, Capability: Output
      - DataSet: 3x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 4: Name: RREFL, Symbol: RAW, Capability: Input
      - DataSet: 2x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    1024
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    1024 (pass-through)
    - Mode 5: Name: RGB I, Symbol: RAW, Capability: Input
      - DataSet: 4x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    1024
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    1024 (pass-through)
    - Mode 6: Name: HSV, Symbol: RAW, Capability: Input
      - DataSet: 3x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     360
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     360 (pass-through)
    - Mode 7: Name: SHSV, Symbol: RAW, Capability: Input
      - DataSet: 4x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     360
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     360 (pass-through)
    - Mode 8: Name: DEBUG, Symbol: RAW, Capability: Input
      - DataSet: 4x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:   65535
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:   65535 (pass-through)
    - Mode 9: Name: CALIB, Symbol: , Capability:
      - DataSet: 7x Int16, TotalFigures: 5, Decimals: 0
        Raw Min:       0, Max:   65535
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:   65535 (pass-through)
````
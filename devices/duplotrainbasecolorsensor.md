# DuploTrainBaseColorSensor

A color sensor attached to the bottom of the DuploTrainBase, used to detected tokens which can then be used to trigger actions.

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Color

Describes how much "color" intensity is detected

**Direction**: Input

**DataType**: sbyte with values between 0-10

### Mode 1 - ColorTag

Describes a discrete list of understood colors which are used as tags on the rails. Without hub connection, the train base links this tags straight to actions in the RgbLight, Motor and Speaker

**Direction**: Input

**DataType**: sbyte (0-10), see dictionary in supplementary definition.

**Notes**
- The ColorTag sensor only works when it is the only mode queried in the port.

### Mode 2 - Reflection

Measures the reflection of light on the surface. The light is emitted by the sensor itself.

**Direction**: Input

**DataType**: sbyte (0-100)

### Mode 3 - RGB

RGB sensor output.

**Direction**: Absolute Output

**DataType**: Short Triplet (red, green, blue) is used with the range 0-10xx.

**Notes**
- The emitted values do not represent the typical 0-255 scale of a rgb component

### 🕵️‍♀️ Mode 4 - Calibration

Calibration of sensor

**Direction**: Input

**DataType**: TODO

**Notes**
- TODO

## Supplementary Definitions

### Color Tags

| Idx | Tag | Color |
| --- | --- | --- |
| -1 | None | n/a |
| 3 | Water | Blue |
| 5 | Redirect | Green |
| 7 | Sound | Yellow |
| 9 | Stop | Red |
| 10 | Light | White |

## Open Questions

- ColorTag only works when queried standalone but not in combined mode. Combined Mode together with e.g. RGB, Reflection and Color detector fails. RGB, Reflection and Color alone works. The combination with the ColorTag mode is advertised.
- RGB sensor emit a range 0-10xx (emitted data is not restricted to 0-1023). Typical RGB representation is 0-255.
- How is calibration be performed?

## Port and Port Mode Information

### DuploTrainBase / Software 0.1.0.0 / Hardware 0.1.0.0

Binary Export

````
06-00-01-0B-06-20
0F-00-04-12-01-2B-00-00-00-00-01-00-00-00-01
0B-00-43-12-01-06-05-1F-00-00-00
07-00-43-12-02-0F-00
11-00-44-12-00-00-43-4F-4C-4F-52-00-00-00-00-00-00
0E-00-44-12-00-01-00-00-00-00-00-00-20-41
0E-00-44-12-00-02-00-00-00-00-00-00-C8-42
0E-00-44-12-00-03-00-00-00-00-00-00-20-41
0A-00-44-12-00-04-69-64-78-00
08-00-44-12-00-05-84-00
0A-00-44-12-00-80-01-00-03-00
11-00-44-12-01-00-43-20-54-41-47-00-00-00-00-00-00
0E-00-44-12-01-01-00-00-00-00-00-00-20-41
0E-00-44-12-01-02-00-00-00-00-00-00-C8-42
0E-00-44-12-01-03-00-00-00-00-00-00-20-41
0A-00-44-12-01-04-69-64-78-00
08-00-44-12-01-05-C4-00
0A-00-44-12-01-80-01-00-03-00
11-00-44-12-02-00-52-45-46-4C-54-00-00-00-00-00-00
0E-00-44-12-02-01-00-00-00-00-00-00-C8-42
0E-00-44-12-02-02-00-00-00-00-00-00-C8-42
0E-00-44-12-02-03-00-00-00-00-00-00-C8-42
0A-00-44-12-02-04-72-61-77-00
08-00-44-12-02-05-10-00
0A-00-44-12-02-80-01-00-03-00
11-00-44-12-03-00-52-47-42-20-49-00-00-00-00-00-00
0E-00-44-12-03-01-00-00-00-00-00-C0-7F-44
0E-00-44-12-03-02-00-00-00-00-00-00-C8-42
0E-00-44-12-03-03-00-00-00-00-00-C0-7F-44
0A-00-44-12-03-04-72-61-77-00
08-00-44-12-03-05-10-00
0A-00-44-12-03-80-03-01-05-00
11-00-44-12-04-00-43-41-4C-49-42-00-00-00-00-00-00
0E-00-44-12-04-01-00-00-00-00-00-00-FA-45
0E-00-44-12-04-02-00-00-00-00-00-00-C8-42
0E-00-44-12-04-03-00-00-00-00-00-00-FA-45
0A-00-44-12-04-04-00-00-00-00
08-00-44-12-04-05-10-00
0A-00-44-12-04-80-03-01-05-00
````

Human Readable Interpretation

````
  - Port: 0x12 / 18
    - IOTypeId: DuploTrainBaseColorSensor / 0x002B / 43
      Revision: SW: 0.1.0.0, HW: 0.1.0.0
      Capabilities: Input LogicalCombinable
      ModeCombinations: [0000000000001111]
    - Mode 0: Name: COLOR, Symbol: idx, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: SupportsNull Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 1: Name: C TAG, Symbol: idx, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: SupportsNull SupportFunctionalMapping20 Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 2: Name: REFLT, Symbol: raw, Capability: Input
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:     100
        Pct Min:       0, Max:     100 (pass-through)
        SI  Min:       0, Max:     100 (pass-through)
    - Mode 3: Name: RGB I, Symbol: raw, Capability: Input
      - DataSet: 3x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    1023
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    1023 (pass-through)
    - Mode 4: Name: CALIB, Symbol: , Capability: Input
      - DataSet: 3x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    8000
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    8000 (pass-through)
````
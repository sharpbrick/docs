# RGB Light

A light emitting LED integrated in hubs which emits colorful light. It can be addressed using RGB colors but also with a pre-defined set of colors

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Discrete Colors

Sets the RGB LED of the hub to a discrete color code defined in a dictionary.

**Direction**: Discrete Output

**DataType**: SByte is used with the range 0-10 (discrete colors; see table below) and 255 for no color

**Notes**
- Percentage has no meaning

### Mode 1 - RGB Colors

Sets the RGB LED of the hub to a RGB encoded color.

**Direction**: Absolute Output

**DataType**: SByte Triplet (red, green, blue) is used with the range 0-255.

**Notes**
- A *Port Input Format Message Setup* has to be sent before to activate the mode.

## Known Related Commands

- PortOutputCommandSetRgbColorNoMessage
- PortOutputCommandSetRgbColorNo2Message

## Supplementary Definitions

### Colors (Mode 0)

| Idx | Color |
| --- | --- |
| 0 | Black |
| 1 | Pink |
| 2 | Purple |
| 3 | Blue |
| 4 | LightBlue |
| 5 | Cyan |
| 6 | Green |
| 7 | Yellow |
| 8 | Orange |
| 9 | Red |
| 10 | White |
| 255 | None |


## Port and Port Mode Information

### MoveHub / Software: 2.0.0.6 / Hardware: 0.1.0.0

Binary Export

````
0B-00-43-32-01-01-02-00-00-03-00
05-00-43-32-02
11-00-44-32-00-00-43-4F-4C-20-4F-00-00-00-00-00-00
0E-00-44-32-00-01-00-00-00-00-00-00-20-41
0E-00-44-32-00-02-00-00-00-00-00-00-C8-42
0E-00-44-32-00-03-00-00-00-00-00-00-20-41
0A-00-44-32-00-04-00-00-00-00
08-00-44-32-00-05-00-44
0A-00-44-32-00-80-01-00-01-00
11-00-44-32-01-00-52-47-42-20-4F-00-00-00-00-00-00
0E-00-44-32-01-01-00-00-00-00-00-00-7F-43
0E-00-44-32-01-02-00-00-00-00-00-00-C8-42
0E-00-44-32-01-03-00-00-00-00-00-00-7F-43
0A-00-44-32-01-04-00-00-00-00
08-00-44-32-01-05-00-10
0A-00-44-32-01-80-03-00-03-00
````

Human Readable Interpretation

````
  Port: 50
    IOTypeId: RgbLight
    HardwareRevision: 0.1.0.0
    SoftwareRevision: 2.0.0.6
    OutputCapability: True
    InputCapability: False
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: COL O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 10
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 10
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: True
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: True
      NumberOfDatasets: 1
      DatasetType: SByte
      TotalFigures: 1
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: RGB O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 255
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 255
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: True
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 3
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````

### TechnicMediumHub / Software: 1.0.0.0 / Hardware: 1.0.0.0

Binary Export

````
0B-00-43-32-01-01-02-00-00-03-00
05-00-43-32-02
11-00-44-32-00-00-43-4F-4C-20-4F-00-00-00-00-00-00
0E-00-44-32-00-01-00-00-00-00-00-00-20-41
0E-00-44-32-00-02-00-00-00-00-00-00-C8-42
0E-00-44-32-00-03-00-00-00-00-00-00-20-41
0A-00-44-32-00-04-00-00-00-00
08-00-44-32-00-05-00-44
0A-00-44-32-00-80-01-00-01-00
11-00-44-32-01-00-52-47-42-20-4F-00-00-00-00-00-00
0E-00-44-32-01-01-00-00-00-00-00-00-7F-43
0E-00-44-32-01-02-00-00-00-00-00-00-C8-42
0E-00-44-32-01-03-00-00-00-00-00-00-7F-43
0A-00-44-32-01-04-00-00-00-00
08-00-44-32-01-05-00-10
0A-00-44-32-01-80-03-00-03-00
````

Human Readable Interpretation

````
  Port: 50
    IOTypeId: RgbLight
    HardwareRevision: 1.0.0.0
    SoftwareRevision: 1.0.0.0
    OutputCapability: True
    InputCapability: False
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: COL O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 10
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 10
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: True
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: True
      NumberOfDatasets: 1
      DatasetType: SByte
      TotalFigures: 1
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: RGB O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 255
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 255
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: True
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 3
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````

### TwoPortHub / Software 1.0.0.0 / Hardware 1.0.0.0

Binary Export

````
0B-00-43-32-01-01-02-00-00-03-00
05-00-43-32-02
12-00-44-32-00-00-43-4F-4C-20-4F-00-00-00-00-00-00-00
0E-00-44-32-00-01-00-00-00-00-00-00-20-41
0E-00-44-32-00-02-00-00-00-00-00-00-C8-42
0E-00-44-32-00-03-00-00-00-00-00-00-20-41
0B-00-44-32-00-04-00-00-00-00-00
08-00-44-32-00-05-00-44
0A-00-44-32-00-80-01-00-01-00
12-00-44-32-01-00-52-47-42-20-4F-00-00-00-00-00-00-00
0E-00-44-32-01-01-00-00-00-00-00-00-7F-43
0E-00-44-32-01-02-00-00-00-00-00-00-C8-42
0E-00-44-32-01-03-00-00-00-00-00-00-7F-43
0B-00-44-32-01-04-00-00-00-00-00
08-00-44-32-01-05-00-10
0A-00-44-32-01-80-03-00-03-00
````

Human Readable Interpretation

````
  Port: 50
    IOTypeId: RgbLight
    HardwareRevision: 1.0.0.0
    SoftwareRevision: 1.0.0.0
    OutputCapability: True
    InputCapability: False
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: COL O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 10
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 10
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: True
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: True
      NumberOfDatasets: 1
      DatasetType: SByte
      TotalFigures: 1
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: RGB O
      IsInput: False
      IsOutput: True
      RawMin: 0
      RawMax: 255
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 255
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: True
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 3
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````

### DuploTrainBaseHub / Software: 0.0.0.1 / Hardware: 0.0.0.1

Binary Export

````
06-00-01-0B-06-20
0F-00-04-11-01-17-00-01-00-00-00-01-00-00-00
0B-00-43-11-01-01-02-00-00-03-00
05-00-43-11-02
11-00-44-11-00-00-43-4F-4C-20-4F-00-00-00-00-00-00
0E-00-44-11-00-01-00-00-00-00-00-00-20-41
0E-00-44-11-00-02-00-00-00-00-00-00-C8-42
0E-00-44-11-00-03-00-00-00-00-00-00-20-41
0A-00-44-11-00-04-00-00-00-00
08-00-44-11-00-05-00-44
0A-00-44-11-00-80-01-00-01-00
11-00-44-11-01-00-52-47-42-20-4F-00-00-00-00-00-00
0E-00-44-11-01-01-00-00-00-00-00-00-7F-43
0E-00-44-11-01-02-00-00-00-00-00-00-C8-42
0E-00-44-11-01-03-00-00-00-00-00-00-7F-43
0A-00-44-11-01-04-00-00-00-00
08-00-44-11-01-05-00-10
0A-00-44-11-01-80-03-00-03-00
````

Human Readable Interpretation

````
  - Port: 0x11 / 17
    - IOTypeId: RgbLight / 0x0017 / 23
      Revision: SW: 0.0.0.1, HW: 0.0.0.1
      Capabilities: Output
      ModeCombinations: []
    - Mode 0: Name: COL O, Symbol: , Capability: Output
      - DataSet: 1x SByte, TotalFigures: 1, Decimals: 0
        Output Mapping: SupportFunctionalMapping20 Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 1: Name: RGB O, Symbol: , Capability: Output
      - DataSet: 3x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Absolute
        Raw Min:       0, Max:     255
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     255 (pass-through)
````
# MarioHubPants

Pants Sensor/Switch on the Mario figure.

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Pants

Number representing the current trousers of Mario.

**Direction**: Input

**DataType**: SByte used as Byte representing Pants.

**Notes**
- Enumeration is likely to extend

## Supplementary Definitions

### Known Pants

| Number | Pants |
| --- | --- |
| 0b00_0000 | None |
| 0b00_1100 | Propeller |
| 0b01_0001 | Cat |
| 0b01_0010 | Fire |
| 0b10_0001 | Normal |
| 0b10_0010 | Builder |

***Note**: Information provided as binary reflecting the micro-switches used for it*.

## Resources

- https://github.com/bricklife/LEGO-Mario-Reveng

## Port and Port Mode Information

### MarioHub / Software x.x.x.x / Hardware x.x.x.x

Binary Export

````
0B-00-43-02-01-02-01-01-00-00-00
05-00-43-02-02
11-00-44-02-00-00-50-41-4E-54-00-00-00-00-00-00-00
0E-00-44-02-00-01-00-00-00-00-00-00-7C-42
0E-00-44-02-00-02-00-00-00-00-00-00-C8-42
0E-00-44-02-00-03-00-00-00-00-00-00-7C-42
0A-00-44-02-00-04-69-64-78-00
08-00-44-02-00-05-84-00
0A-00-44-02-00-80-01-00-03-00
````

Human Readable Interpretation

````
  Port: 2
    IOTypeId: 74
    HardwareRevision: 2.0.0.0
    SoftwareRevision: 0.0.0.1
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: PANT
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 63
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 63
      Symbol: idx
      InputSupportsNull: True
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: False
      InputDiscrete: True
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
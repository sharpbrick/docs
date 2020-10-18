# MarioHubTagSensor

Barcode and Color scanner.

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Tag Sensor

Scans a colorful barcode, decode it into a number. Additionally delivers a pre-defined color enumeration.

**Direction**: Input

**DataType**: First Int16 representing a scanned number from a barcode (see enumeration), Second Int16 represent a pre-defined color (see enumeration).

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).
- Enumeration is likely to extend.

### Mode 1 - RGB Sensor

Scans a color.

**Direction**: Input

**DataType**: SByte Triplet interpreted as Byte Triplet (r, g, b). 

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

## Supplementary Definitions

### Known Barcodes

| Nr | Known Item |
| --- | --- |
| 0xFFFF | None |
| 0x0002 | Goomba |
| 0x0014 | Refresh |
| 0x0029 | Question |
| 0x002E | Cloud |
| 0x0079 | Bat |
| 0x007B | Star |
| 0x0088 | KingBoo |
| 0x0099 | BowserJr |
| 0x00B7 | BowserGoal |
| 0x00B8 | Pipe |

### Known Barcodes

| Nr | Known Color |
| --- | --- |
| 0xFFFF | None |
| 0x0013 | White |
| 0x0015 | Red |
| 0x0017 | Blue |
| 0x0018 | Yellow |
| 0x001A | Black |
| 0x0025 | Green |
| 0x006A | Brown |
| 0x010C | Unknown1 |
| 0x0138 | Unknown2 |
| 0x0142 | Cyan |

## Open Questions

- Complete List of Barcodes & Colors

## Resources

- https://github.com/bricklife/LEGO-Mario-Reveng

## Port and Port Mode Information

### MarioHub / Software 0.0.0.1 / Hardware 2.0.0.0

Binary Export

````
0B-00-43-01-01-06-02-03-00-00-00
07-00-43-01-02-03-00
11-00-44-01-00-00-54-41-47-00-00-00-00-00-00-00-00
0E-00-44-01-00-01-00-00-00-00-00-00-20-41
0E-00-44-01-00-02-00-00-00-00-00-00-C8-42
0E-00-44-01-00-03-00-00-00-00-00-00-20-41
0A-00-44-01-00-04-69-64-78-00
08-00-44-01-00-05-84-00
0A-00-44-01-00-80-02-01-03-00
11-00-44-01-01-00-52-47-42-00-00-00-00-00-00-00-00
0E-00-44-01-01-01-00-00-00-00-00-00-20-41
0E-00-44-01-01-02-00-00-00-00-00-00-C8-42
0E-00-44-01-01-03-00-00-00-00-00-00-20-41
0A-00-44-01-01-04-72-61-77-00
08-00-44-01-01-05-84-00
0A-00-44-01-01-80-03-00-03-00
````

Human Readable Interpretation

````
  Port: 1
    IOTypeId: 73
    HardwareRevision: 2.0.0.0
    SoftwareRevision: 0.0.0.1
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: True
    LogicalSynchronizableCapability: False
    ModeCombinations: [0000000000000011]
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: TAG
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 10
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 10
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
      NumberOfDatasets: 2
      DatasetType: Int16
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: RGB
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 10
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 10
      Symbol: raw
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
      NumberOfDatasets: 3
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
# TechnicMediumHubGestureSensor

Detects a series of Gestures

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Gestures

Gestures

**Direction**: Input

**DataType**: SByte (positive values) representing a value of the Gesture Enumeration (see below)

## Supplementary Definitions

### Gestures Enumeration

| # | Name | Assumed Gesture |
| --- | --- | --- |
| 0 | None | None |
| 1 | Gesture1 | Tap |
| 2 | Gesture2 | maybe Bounce |
| 3 | Gesture3 | maybe Shake |
| 4 | Gesture4 | FreeFall |

## Open Questions

- Exact Gesture Mapping [1](https://bricks.stackexchange.com/questions/15271/technic-medium-hub-supported-gestures-of-gesture-recognition-sensor), [2](https://github.com/sharpbrick/powered-up/issues/90)

## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
0B-00-43-64-01-02-01-01-00-00-00
05-00-43-64-02
11-00-44-64-00-00-47-45-53-54-00-00-00-00-00-00-00
0E-00-44-64-00-01-00-00-00-00-00-00-80-40
0E-00-44-64-00-02-00-00-00-00-00-00-C8-42
0E-00-44-64-00-03-00-00-00-00-00-00-80-40
0A-00-44-64-00-04-00-00-00-00
08-00-44-64-00-05-44-00
0A-00-44-64-00-80-01-00-01-00
````

Human Readable Interpretation

````
  Port: 100
    IOTypeId: TechnicMediumHubGestureSensor
    HardwareRevision: 0.0.0.1
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
      Name: GEST
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 4
      Symbol:
      InputSupportsNull: False
      InputSupportFunctionalMapping20: True
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
      TotalFigures: 1
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
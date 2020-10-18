# MarioHubAccelerometer

Measures Gestures and Impacts using an accelerometer.

**Type**: Hub Device

**Status**: Exploration

## Modes

### Mode 0 - Impacts

Detected impacts to the device.

**Direction**: Input

**DataType**: SByte Triplet (x,y,z) of unit cnt. Counting the impacts in each dimension.

**Notes**
- ⚠ This mode is a speculative

### Mode 1 - Gestures

Detects a gesture using the accelerometer.

**Direction**: Input

**DataType**: Int16 representing a well-known gesture.

**Notes**
- TODO

## Supplementary Definitions

### Gesture Enumeration

Maybe, see [TechnicMediumHubGestureSensor](technicmediumhub-gesturesensor.md).

## Open Questions

- Is it impact counting? (would make sense for a LEGO figure jumping around)
- Is it Gesture recognition? (would make sense for a small figure)

## Resources

- https://github.com/bricklife/LEGO-Mario-Reveng

## Port and Port Mode Information

### MarioHub / Software 0.0.0.1 / Hardware 2.0.0.0

Binary Export

````
0B-00-43-00-01-06-02-03-00-00-00
07-00-43-00-02-03-00
11-00-44-00-00-00-52-41-57-00-00-00-00-00-00-00-00
0E-00-44-00-00-01-00-00-00-00-00-00-C8-42
0E-00-44-00-00-02-00-00-00-00-00-00-C8-42
0E-00-44-00-00-03-00-00-00-00-00-00-C8-42
0A-00-44-00-00-04-63-6E-74-00
08-00-44-00-00-05-84-00
0A-00-44-00-00-80-03-00-03-00
11-00-44-00-01-00-47-45-53-54-00-00-00-00-00-00-00
0E-00-44-00-01-01-00-00-00-00-00-00-C8-42
0E-00-44-00-01-02-00-00-00-00-00-00-C8-42
0E-00-44-00-01-03-00-00-00-00-00-00-C8-42
0A-00-44-00-01-04-63-6E-74-00
08-00-44-00-01-05-84-00
0A-00-44-00-01-80-02-01-03-00
````

Human Readable Interpretation

````
  Port: 0
    IOTypeId: 71
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
      Name: RAW
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 100
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 100
      Symbol: cnt
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
    Mode: 1
      Name: GEST
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 100
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 100
      Symbol: cnt
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
````
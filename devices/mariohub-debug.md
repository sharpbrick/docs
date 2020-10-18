# MarioHubDebug

Debug Interface to MarioHub

**Type**: Hub Device

**Status**: Exploration

## Modes

### Mode 0 - TODO

TODO Description

**Direction**: Input | Output

**DataType**: TODO

**Notes**
- TODO

### Mode 1 - TODO

TODO Description

**Direction**: Input | Output

**DataType**: TODO

**Notes**
- TODO

## Supplementary Definitions

### some stuff

lists or other things

## Open Questions

- Everything

## Resources

- https://github.com/bricklife/LEGO-Mario-Reveng

## Port and Port Mode Information

### MarioHub / Software 0.0.0.1 / Hardware 2.0.0.0

Binary Export

````
0B-00-43-03-01-02-04-0F-00-00-00
05-00-43-03-02
11-00-44-03-00-00-43-48-41-4C-00-00-00-00-00-00-00
0E-00-44-03-00-01-00-00-00-00-00-FF-7F-47
0E-00-44-03-00-02-00-00-00-00-00-00-C8-42
0E-00-44-03-00-03-00-00-00-00-00-FF-7F-47
0A-00-44-03-00-04-6E-61-00-00
08-00-44-03-00-05-84-00
0A-00-44-03-00-80-02-01-03-00
11-00-44-03-01-00-56-45-52-53-00-00-00-00-00-00-00
0E-00-44-03-01-01-00-00-00-00-00-00-7F-43
0E-00-44-03-01-02-00-00-00-00-00-00-C8-42
0E-00-44-03-01-03-00-00-00-00-00-00-7F-43
0A-00-44-03-01-04-6E-61-00-00
08-00-44-03-01-05-84-00
0A-00-44-03-01-80-04-02-0A-00
11-00-44-03-02-00-45-56-45-4E-54-53-00-00-00-00-00
0E-00-44-03-02-01-00-00-00-00-00-FF-7F-47
0E-00-44-03-02-02-00-00-00-00-00-00-C8-42
0E-00-44-03-02-03-00-00-00-00-00-FF-7F-47
0A-00-44-03-02-04-6E-61-00-00
08-00-44-03-02-05-84-00
0A-00-44-03-02-80-02-01-0A-00
11-00-44-03-03-00-44-45-42-55-47-00-00-00-00-00-00
0E-00-44-03-03-01-00-00-00-00-00-FF-7F-47
0E-00-44-03-03-02-00-00-00-00-00-00-C8-42
0E-00-44-03-03-03-00-00-00-00-00-FF-7F-47
0A-00-44-03-03-04-6E-61-00-00
08-00-44-03-03-05-84-00
0A-00-44-03-03-80-04-02-0A-00
````

Human Readable Interpretation

````
  Port: 3
    IOTypeId: 70
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
      Name: CHAL
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 65535
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 65535
      Symbol: na
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
      Name: VERS
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 255
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 255
      Symbol: na
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
      NumberOfDatasets: 4
      DatasetType: Int32
      TotalFigures: 10
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 2
      Name: EVENTS
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 65535
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 65535
      Symbol: na
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
      TotalFigures: 10
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 3
      Name: DEBUG
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 65535
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 65535
      Symbol: na
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
      NumberOfDatasets: 4
      DatasetType: Int32
      TotalFigures: 10
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
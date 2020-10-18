# Current

Allows to measure the energy consumption of a hub.

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Current Load

Indicates the current currently utilized.

**Direction**: Input

**DataType**: Int16 (positive values) representing mA

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

### Mode 1 - Current Supply

Indicates the current currently supply.

**Direction**: Input

**DataType**: Int16 (positive values) representing mA

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

## Open Issues

- Whether the L within CUR L stands for load is currently a speculation [1](https://bricks.stackexchange.com/questions/15107/technic-medium-hub-what-is-the-difference-between-voltage-l-and-s), [2](https://github.com/sharpbrick/powered-up/issues/29)

## Port and Port Mode Information

### MoveHub / Software: 0.0.1.0 / Hardware: 0.0.0.2

Binary Export

````
0B-00-43-3B-01-02-02-03-00-00-00
05-00-43-3B-02
11-00-44-3B-00-00-43-55-52-20-4C-00-00-00-00-00-00
0E-00-44-3B-00-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-00-03-00-00-00-00-00-C0-18-45
0A-00-44-3B-00-04-6D-41-00-00
08-00-44-3B-00-05-10-00
0A-00-44-3B-00-80-01-01-04-00
11-00-44-3B-01-00-43-55-52-20-53-00-00-00-00-00-00
0E-00-44-3B-01-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-01-03-00-00-00-00-00-C0-18-45
0A-00-44-3B-01-04-6D-41-00-00
08-00-44-3B-01-05-10-00
0A-00-44-3B-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 59
    IOTypeId: Current
    HardwareRevision: 0.0.0.2
    SoftwareRevision: 0.0.1.0
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: CUR L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 2444
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: CUR S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 2444
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````


### TechnicMediumHub / Software: 1.0.0.0 / Hardware: 1.0.0.0

Binary Export

````
0B-00-43-3B-01-02-02-03-00-00-00
05-00-43-3B-02
11-00-44-3B-00-00-43-55-52-20-4C-00-00-00-00-00-00
0E-00-44-3B-00-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-00-03-00-00-00-00-00-78-82-45
0A-00-44-3B-00-04-6D-41-00-00
08-00-44-3B-00-05-10-00
0A-00-44-3B-00-80-01-01-04-00
11-00-44-3B-01-00-43-55-52-20-53-00-00-00-00-00-00
0E-00-44-3B-01-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-01-03-00-00-00-00-00-78-82-45
0A-00-44-3B-01-04-6D-41-00-00
08-00-44-3B-01-05-10-00
0A-00-44-3B-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 59
    IOTypeId: Current
    HardwareRevision: 1.0.0.0
    SoftwareRevision: 1.0.0.0
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: CUR L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 4175
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: CUR S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 4175
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````

### TwoPortHub / Software 0.0.0.2 / Hardware 0.0.0.2

Binary Export

````
0B-00-43-3B-01-02-02-03-00-00-00
05-00-43-3B-02
12-00-44-3B-00-00-43-55-52-20-4C-00-00-00-00-00-00-00
0E-00-44-3B-00-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-00-03-00-00-00-00-00-C0-18-45
0B-00-44-3B-00-04-6D-41-00-00-00
08-00-44-3B-00-05-10-00
0A-00-44-3B-00-80-01-01-04-00
12-00-44-3B-01-00-43-55-52-20-53-00-00-00-00-00-00-00
0E-00-44-3B-01-01-00-00-00-00-00-F0-7F-45
0E-00-44-3B-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3B-01-03-00-00-00-00-00-C0-18-45
0B-00-44-3B-01-04-6D-41-00-00-00
08-00-44-3B-01-05-10-00
0A-00-44-3B-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 59
    IOTypeId: Current
    HardwareRevision: 0.0.0.2
    SoftwareRevision: 0.0.0.2
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: CUR L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 2444
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: CUR S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 2444
      Symbol: mA
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 4
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````

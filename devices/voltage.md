# Voltage

Allows to measure the available voltage of the batteries within an hub.

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Voltage Load

Indicates the voltage currently utilized.

**Direction**: Input

**DataType**: Int16 (positive values) representing mV

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

### Mode 1 - Voltage Supply

Indicates the voltage currently supplied.

**Direction**: Input

**DataType**: Int16 (positive values) representing mV

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

## Open Issues

- Whether the S within VLT L stands for load is currently a speculation [1](https://bricks.stackexchange.com/questions/15107/technic-medium-hub-what-is-the-difference-between-voltage-l-and-s), [2](https://github.com/sharpbrick/powered-up/issues/29)

## Port and Port Mode Information

### MarioHub / Software: 2.0.0.0 / Hardware: 0.0.0.1

Binary Export

````
0B-00-43-06-01-02-02-03-00-00-00
05-00-43-06-02
11-00-44-06-00-00-56-4C-54-20-4C-00-00-00-00-00-00
0E-00-44-06-00-01-00-00-00-00-00-10-29-45
0E-00-44-06-00-02-00-00-00-00-00-00-C8-42
0E-00-44-06-00-03-00-00-00-00-00-40-4E-45
0A-00-44-06-00-04-6D-56-00-00
08-00-44-06-00-05-10-00
0A-00-44-06-00-80-01-01-04-00
11-00-44-06-01-00-56-4C-54-20-53-00-00-00-00-00-00
0E-00-44-06-01-01-00-00-00-00-00-10-29-45
0E-00-44-06-01-02-00-00-00-00-00-00-C8-42
0E-00-44-06-01-03-00-00-00-00-00-40-4E-45
0A-00-44-06-01-04-6D-56-00-00
08-00-44-06-01-05-10-00
0A-00-44-06-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 6
    IOTypeId: Voltage
    HardwareRevision: 0.0.0.1
    SoftwareRevision: 2.0.0.0
    OutputCapability: False
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: VLT L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 2705
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 3300
      Symbol: mV
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
      Name: VLT S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 2705
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 3300
      Symbol: mV
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

### MoveHub / Software 0.0.1.0 / Hardware 0.0.0.2

Binary Export

````
0B-00-43-3C-01-02-02-03-00-00-00
05-00-43-3C-02
11-00-44-3C-00-00-56-4C-54-20-4C-00-00-00-00-00-00
0E-00-44-3C-00-01-00-00-00-00-00-50-73-45
0E-00-44-3C-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-00-03-00-00-00-00-00-00-16-46
0A-00-44-3C-00-04-6D-56-00-00
08-00-44-3C-00-05-10-00
0A-00-44-3C-00-80-01-01-04-00
11-00-44-3C-01-00-56-4C-54-20-53-00-00-00-00-00-00
0E-00-44-3C-01-01-00-00-00-00-00-50-73-45
0E-00-44-3C-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-01-03-00-00-00-00-00-00-16-46
0A-00-44-3C-01-04-6D-56-00-00
08-00-44-3C-01-05-10-00
0A-00-44-3C-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 60
    IOTypeId: Voltage
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
      Name: VLT L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 3893
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9600
      Symbol: mV
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
      Name: VLT S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 3893
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9600
      Symbol: mV
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
0B-00-43-3C-01-02-02-03-00-00-00
05-00-43-3C-02
11-00-44-3C-00-00-56-4C-54-20-4C-00-00-00-00-00-00
0E-00-44-3C-00-01-00-00-00-00-00-F0-7F-45
0E-00-44-3C-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-00-03-00-00-00-00-00-3C-16-46
0A-00-44-3C-00-04-6D-56-00-00
08-00-44-3C-00-05-10-00
0A-00-44-3C-00-80-01-01-04-00
11-00-44-3C-01-00-56-4C-54-20-53-00-00-00-00-00-00
0E-00-44-3C-01-01-00-00-00-00-00-F0-7F-45
0E-00-44-3C-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-01-03-00-00-00-00-00-3C-16-46
0A-00-44-3C-01-04-6D-56-00-00
08-00-44-3C-01-05-10-00
0A-00-44-3C-01-80-01-01-04-00
````

Human Readable Interpretation

````
Port: 60
    IOTypeId: Voltage
    HardwareRevision: 1.0.0.0
    SoftwareRevision: 1.0.0.0
    OutputCapability: True
    InputCapability: False
    LogicalCombinableCapability: True
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: VLT L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9615
      Symbol: mV
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
      Name: VLT S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 4095
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9615
      Symbol: mV
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
0B-00-43-3C-01-02-02-03-00-00-00
05-00-43-3C-02
12-00-44-3C-00-00-56-4C-54-20-4C-00-00-00-00-00-00-00
0E-00-44-3C-00-01-00-00-00-00-00-50-73-45
0E-00-44-3C-00-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-00-03-00-00-00-00-00-00-16-46
0B-00-44-3C-00-04-6D-56-00-00-00
08-00-44-3C-00-05-10-00
0A-00-44-3C-00-80-01-01-04-00
12-00-44-3C-01-00-56-4C-54-20-53-00-00-00-00-00-00-00
0E-00-44-3C-01-01-00-00-00-00-00-50-73-45
0E-00-44-3C-01-02-00-00-00-00-00-00-C8-42
0E-00-44-3C-01-03-00-00-00-00-00-00-16-46
0B-00-44-3C-01-04-6D-56-00-00-00
08-00-44-3C-01-05-10-00
0A-00-44-3C-01-80-01-01-04-00
````

Human Readable Interpretation

````
  Port: 60
    IOTypeId: Voltage
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
      Name: VLT L
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 3893
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9600
      Symbol: mV
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
      Name: VLT S
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 3893
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 9600
      Symbol: mV
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

### DuploTrainBaseHub / Software: 0.0.0.1 / Hardware: 0.0.0.1

Binary Export

````
06-00-01-0B-06-20
0F-00-04-14-01-14-00-01-00-00-00-01-00-00-00
0B-00-43-14-01-02-02-03-00-00-00
05-00-43-14-02
11-00-44-14-00-00-56-4C-54-20-4C-00-00-00-00-00-00
0E-00-44-14-00-01-00-00-00-00-00-70-3E-45
0E-00-44-14-00-02-00-00-00-00-00-00-C8-42
0E-00-44-14-00-03-00-00-00-00-00-00-C8-45
0A-00-44-14-00-04-6D-56-00-00
08-00-44-14-00-05-10-00
0A-00-44-14-00-80-01-01-04-00
11-00-44-14-01-00-56-4C-54-20-53-00-00-00-00-00-00
0E-00-44-14-01-01-00-00-00-00-00-70-3E-45
0E-00-44-14-01-02-00-00-00-00-00-00-C8-42
0E-00-44-14-01-03-00-00-00-00-00-00-C8-45
0A-00-44-14-01-04-6D-56-00-00
08-00-44-14-01-05-10-00
0A-00-44-14-01-80-01-01-04-00
````

Human Readable Interpretation

````
  - Port: 0x14 / 20
    - IOTypeId: Voltage / 0x0014 / 20
      Revision: SW: 0.0.0.1, HW: 0.0.0.1
      Capabilities: Input
      ModeCombinations: []
    - Mode 0: Name: VLT L, Symbol: mV, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    3047
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    6400 (scaling)
    - Mode 1: Name: VLT S, Symbol: mV, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Raw Min:       0, Max:    3047
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    6400 (scaling)
````
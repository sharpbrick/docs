# TechnicMediumHubTiltSensor

Sensor to detect the angle of the device in all dimensions and to detect impacts.

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Angular Position

The Angular Position of the device (as orientation is configured).

**Direction**: Input

**DataType**: Int16 triplet (x,y,z) representing degrees (-180, 180)

### Mode 1 - Impacts

Impact counts (based against thresholds and bumpoff configuration)

**Direction**: Input

**DataType**: Int32 triplet (x,y,z) representing impacts counts (can be reset).

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

### Mode 2 - Configuration

TODO Description

**Direction**: Output

**DataType**: SByte tuple.

## Known Related Commands

- TiltImpactPresetAsync
- PortOutputCommandTiltConfigImpactMessage
- PortOutputCommandTiltConfigOrientationMessage

## Supplementary Definitions

### Device Orientation

| Idx | Color |
| --- | --- |
| 0 | Bottom |
| 1 | Front |
| 2 | Back |
| 3 | Left |
| 4 | Right |
| 5 | Top |
| 6 | UseActualAsBottomReference |

## Open Questions

- Definition of Configuration Mode


## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
0B-00-43-63-01-03-03-03-00-04-00
05-00-43-63-02
11-00-44-63-00-00-50-4F-53-00-00-00-00-00-00-00-00
0E-00-44-63-00-01-00-00-34-C3-00-00-34-43
0E-00-44-63-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-63-00-03-00-00-34-C3-00-00-34-43
0A-00-44-63-00-04-44-45-47-00
08-00-44-63-00-05-50-00
0A-00-44-63-00-80-03-01-03-00
11-00-44-63-01-00-49-4D-50-00-00-00-00-00-00-00-00
0E-00-44-63-01-01-00-00-00-00-00-00-C8-42
0E-00-44-63-01-02-00-00-00-00-00-00-C8-42
0E-00-44-63-01-03-00-00-00-00-00-00-C8-42
0A-00-44-63-01-04-43-4E-54-00
08-00-44-63-01-05-08-00
0A-00-44-63-01-80-01-02-03-00
11-00-44-63-02-00-43-46-47-00-00-00-00-00-00-00-00
0E-00-44-63-02-01-00-00-00-00-00-00-7F-43
0E-00-44-63-02-02-00-00-00-00-00-00-C8-42
0E-00-44-63-02-03-00-00-00-00-00-00-7F-43
0A-00-44-63-02-04-00-00-00-00
08-00-44-63-02-05-00-10
0A-00-44-63-02-80-02-00-03-00
````

Human Readable Interpretation

````
  Port: 99
    IOTypeId: TechnicMediumHubTiltSensor
    HardwareRevision: 0.0.0.1
    SoftwareRevision: 0.0.0.1
    OutputCapability: True
    InputCapability: True
    LogicalCombinableCapability: False
    LogicalSynchronizableCapability: False
    ModeCombinations: []
    UsedCombinationIndex: 0
    MultiUpdateEnabled: False
    ConfiguredModeDataSetIndex: []
    Mode: 0
      Name: POS
      IsInput: True
      IsOutput: False
      RawMin: -180
      RawMax: 180
      PctMin: -100
      PctMax: 100
      SIMin: -180
      SIMax: 180
      Symbol: DEG
      InputSupportsNull: False
      InputSupportFunctionalMapping20: True
      InputAbsolute: True
      InputRelative: False
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 3
      DatasetType: Int16
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 1
      Name: IMP
      IsInput: True
      IsOutput: False
      RawMin: 0
      RawMax: 100
      PctMin: 0
      PctMax: 100
      SIMin: 0
      SIMax: 100
      Symbol: CNT
      InputSupportsNull: False
      InputSupportFunctionalMapping20: False
      InputAbsolute: False
      InputRelative: True
      InputDiscrete: False
      OutputSupportsNull: False
      OutputSupportFunctionalMapping20: False
      OutputAbsolute: False
      OutputRelative: False
      OutputDiscrete: False
      NumberOfDatasets: 1
      DatasetType: Int32
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
    Mode: 2
      Name: CFG
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
      NumberOfDatasets: 2
      DatasetType: SByte
      TotalFigures: 3
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
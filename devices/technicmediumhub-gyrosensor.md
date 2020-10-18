# TechnicMediumHubGyroSensor

A sensor detecting rotation speed of the device. As a consequence gyroscopes **measure rotation** to the position in space

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Rotation

Rotation speed of the hub

**Direction**: Input

**DataType**: Int16 triplets (x, y, z) representing DPS (degress per second). For a actual degree of the device, see the `TechnicMediumHubTiltSensor`.

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
0B-00-43-62-01-02-01-01-00-00-00
05-00-43-62-02
11-00-44-62-00-00-52-4F-54-00-00-00-00-00-00-00-00
0E-00-44-62-00-01-D7-36-DF-C6-D7-36-DF-46
0E-00-44-62-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-62-00-03-00-00-FA-C4-00-00-FA-44
0A-00-44-62-00-04-44-50-53-00
08-00-44-62-00-05-50-00
0A-00-44-62-00-80-03-01-03-00
````

Human Readable Interpretation

````
  Port: 98
    IOTypeId: TechnicMediumHubGyroSensor
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
      Name: ROT
      IsInput: True
      IsOutput: False
      RawMin: -28571,42
      RawMax: 28571,42
      PctMin: -100
      PctMax: 100
      SIMin: -2000
      SIMax: 2000
      Symbol: DPS
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
````
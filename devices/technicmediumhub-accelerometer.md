# TechnicMediumHubAccelerometer

A sensor measuring the change in gravity as detected in the device. As a consequence accelerometers **measure translation** to the position in space

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### Mode 0 - Gravity Sensor

Gravity as measured in four dimensions

**Direction**: Input

**DataType**: Int16 triplet (x,y,z) representing gravity in mG

**Notes**
- ⚠ [Scaling of Raw/SI](../lwp/note-value-scaling.md).

### Mode 1 - Calibration

Calibration of sensor

**Direction**: Input

**DataType**: TODO

**Notes**
- TODO

## Open Questions

- How is calibration be performed? [1](https://github.com/sharpbrick/powered-up/issues/30)


## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
0B-00-43-61-01-02-02-03-00-00-00
05-00-43-61-02
11-00-44-61-00-00-47-52-56-00-00-00-00-00-00-00-00
0E-00-44-61-00-01-00-00-00-C7-00-00-00-47
0E-00-44-61-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-61-00-03-00-00-FA-C5-00-00-FA-45
0A-00-44-61-00-04-6D-47-00-00
08-00-44-61-00-05-50-00
0A-00-44-61-00-80-03-01-03-00
11-00-44-61-01-00-43-41-4C-00-00-00-00-00-00-00-00
0E-00-44-61-01-01-00-00-80-3F-00-00-80-3F
0E-00-44-61-01-02-00-00-C8-C2-00-00-C8-42
0E-00-44-61-01-03-00-00-80-3F-00-00-80-3F
0A-00-44-61-01-04-00-00-00-00
08-00-44-61-01-05-50-00
0A-00-44-61-01-80-01-00-00-00
````

Human Readable Interpretation

````
  Port: 97
    IOTypeId: TechnicMediumHubAccelerometer
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
      Name: GRV
      IsInput: True
      IsOutput: False
      RawMin: -32768
      RawMax: 32768
      PctMin: -100
      PctMax: 100
      SIMin: -8000
      SIMax: 8000
      Symbol: mG
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
      Name: CAL
      IsInput: True
      IsOutput: False
      RawMin: 1
      RawMax: 1
      PctMin: -100
      PctMax: 100
      SIMin: 1
      SIMax: 1
      Symbol:
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
      NumberOfDatasets: 1
      DatasetType: SByte
      TotalFigures: 0
      Decimals: 0
      DeltaInterval: 0
      NotificationEnabled: False
````
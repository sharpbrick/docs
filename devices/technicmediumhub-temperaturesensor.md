# TechnicMediumHubTemperatureSensor

Temperature sensor as part of the `TechnicMediumHub`.

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Temperature in °C

Reports the current temperature of the device

**Direction**: Input

**DataType**: Int16 representing °C with one decimal place.

## Open Questions

- Why there are two temperature sensors in `TechnicMediumHub` only diffing by parallel installation? Old/New Software for Testing purposes? [1](https://github.com/sharpbrick/powered-up/issues/31)


## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1 / Hardware 0.0.0.1  

Binary Export

````
0B-00-43-60-01-02-01-01-00-00-00
05-00-43-60-02
11-00-44-60-00-00-54-45-4D-50-00-00-00-00-00-00-00
0E-00-44-60-00-01-00-00-61-C4-00-00-61-44
0E-00-44-60-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-60-00-03-00-00-B4-C2-00-00-B4-42
0A-00-44-60-00-04-44-45-47-00
08-00-44-60-00-05-50-00
0A-00-44-60-00-80-01-01-05-01
````

Human Readable Interpretation

````
  Port: 96
    IOTypeId: TechnicMediumHubTemperatureSensor
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
      Name: TEMP
      IsInput: True
      IsOutput: False
      RawMin: -900
      RawMax: 900
      PctMin: -100
      PctMax: 100
      SIMin: -90
      SIMax: 90
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
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 5
      Decimals: 1
      DeltaInterval: 0
      NotificationEnabled: False
````


### TechnicMediumHub / Software 1.0.0.0 / Hardware 1.0.0.0

Binary Export

````
0B-00-43-3D-01-02-01-01-00-00-00
05-00-43-3D-02
11-00-44-3D-00-00-54-45-4D-50-00-00-00-00-00-00-00
0E-00-44-3D-00-01-00-00-61-C4-00-00-61-44
0E-00-44-3D-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-3D-00-03-00-00-B4-C2-00-00-B4-42
0A-00-44-3D-00-04-44-45-47-00
08-00-44-3D-00-05-50-00
0A-00-44-3D-00-80-01-01-05-01
````

Human Readable Interpretation

````
  Port: 61
    IOTypeId: TechnicMediumHubTemperatureSensor
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
      Name: TEMP
      IsInput: True
      IsOutput: False
      RawMin: -900
      RawMax: 900
      PctMin: -100
      PctMax: 100
      SIMin: -90
      SIMax: 90
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
      NumberOfDatasets: 1
      DatasetType: Int16
      TotalFigures: 5
      Decimals: 1
      DeltaInterval: 0
      NotificationEnabled: False
````
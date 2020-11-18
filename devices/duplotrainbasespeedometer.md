# DuploTrainBaseSpeedometer

Different to external tacho motors (e.g. the Technic Motors), the tacho of the DuploTrainBase is a separatae port. It measures the speed and the position relative to a starting point.

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Speed

Speed of the related [DuploTrainBaseMotor](duplotrainbasemotor.md).

**Direction**: Input

**DataType**: Int16

### Mode 1 - Count

Distance from starting point [DuploTrainBaseMotor](duplotrainbasemotor.md). Increments and Decrements ongoingly.

**Direction**: Input

**DataType**: int

**Notes**
- ⚠ The Count Mode is ill-defined when queried using the LWP. A singular value 8-8 does [not scale](../lwp/note-value-scaling.md). Percentage and SI scaling cannot be applied.

## Open Questions

- What units do speed and count have.

## Port and Port Mode Information

### DuploTrainBaseHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
06-00-01-0B-06-20
0F-00-04-13-01-2C-00-01-00-00-00-01-00-00-00
0B-00-43-13-01-06-03-07-00-00-00
07-00-43-13-02-03-00
11-00-44-13-00-00-53-50-45-45-44-00-00-00-00-00-00
0E-00-44-13-00-01-00-00-96-C3-00-00-96-43
0E-00-44-13-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-13-00-03-00-00-20-C1-00-00-20-41
0A-00-44-13-00-04-73-70-64-00
08-00-44-13-00-05-50-00
0A-00-44-13-00-80-01-01-05-00
11-00-44-13-01-00-43-4F-55-4E-54-00-00-00-00-00-00
0E-00-44-13-01-01-00-00-00-41-00-00-00-41
0E-00-44-13-01-02-00-00-C8-C2-00-00-C8-42
0E-00-44-13-01-03-00-00-B4-43-00-00-B4-43
0A-00-44-13-01-04-63-6E-74-00
08-00-44-13-01-05-08-00
0A-00-44-13-01-80-01-02-04-00
11-00-44-13-02-00-43-41-4C-49-42-00-00-00-00-00-00
0E-00-44-13-02-01-00-00-00-00-00-00-80-45
0E-00-44-13-02-02-00-00-00-00-00-00-C8-42
0E-00-44-13-02-03-00-00-00-00-00-00-80-45
0A-00-44-13-02-04-6E-2F-61-00
08-00-44-13-02-05-08-00
0A-00-44-13-02-80-04-01-05-00
````

Human Readable Interpretation

````
  - Port: 0x13 / 19
    - IOTypeId: DuploTrainBaseSpeedometer / 0x002C / 44
      Revision: SW: 0.0.0.1, HW: 0.0.0.1
      Capabilities: Input LogicalCombinable
      ModeCombinations: [0000000000000011]
    - Mode 0: Name: SPEED, Symbol: spd, Capability: Input
      - DataSet: 1x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: SupportFunctionalMapping20 Absolute
        Raw Min:    -300, Max:     300
        Pct Min:    -100, Max:     100 (scaling)
        SI  Min:     -10, Max:      10 (scaling)
    - Mode 1: Name: COUNT, Symbol: cnt, Capability: Input
      - DataSet: 1x Int32, TotalFigures: 4, Decimals: 0
        Input Mapping: Relative
        Raw Min:       8, Max:       8
        Pct Min:    -100, Max:     100 (scaling)
        SI  Min:     360, Max:     360 (scaling, translation)
    - Mode 2: Name: CALIB, Symbol: n/a, Capability: Input
      - DataSet: 4x Int16, TotalFigures: 5, Decimals: 0
        Input Mapping: Relative
        Raw Min:       0, Max:    4096
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:    4096 (pass-through)
````
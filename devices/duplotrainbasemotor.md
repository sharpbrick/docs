# DuploTrainBaseMotor

Internal Motor on the DuploTrainBase

**Type**: Hub Device

**Status**: Well Defined

## Modes

### Mode 0 - Speed

Speed control of the motor

**Direction**: Output

**DataType**: Int8 (in range-100 - 100)

### Mode 1 - Seconds On (as in running)

Seconds activated.

**Direction**: Input

**DataType**: Int32

## Known Related Commands

- PortOutputCommandStartPowerMessage

## Port and Port Mode Information

### DuploTrainBaseHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
06-00-01-0B-06-20
0F-00-04-00-01-29-00-01-00-00-00-01-00-00-00
0B-00-43-00-01-03-02-02-00-01-00
05-00-43-00-02
11-00-44-00-00-00-54-20-4D-4F-54-00-00-00-00-00-00
0E-00-44-00-00-01-00-00-C8-C2-00-00-C8-42
0E-00-44-00-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-00-00-03-00-00-C8-C2-00-00-C8-42
0A-00-44-00-00-04-70-77-72-00
08-00-44-00-00-05-00-50
0A-00-44-00-00-80-01-00-03-00
11-00-44-00-01-00-4F-4E-53-45-43-00-00-00-00-00-00
0E-00-44-00-01-01-00-00-00-00-00-00-80-3F
0E-00-44-00-01-02-00-00-00-00-00-00-C8-42
0E-00-44-00-01-03-00-00-00-00-00-00-80-3F
0A-00-44-00-01-04-73-65-63-00
08-00-44-00-01-05-08-00
0A-00-44-00-01-80-01-02-04-00
````

Human Readable Interpretation

````
  - Port: 0x00 / 0
    - IOTypeId: DuploTrainBaseMotor / 0x0029 / 41
      Revision: SW: 0.0.0.1, HW: 0.0.0.1
      Capabilities: Output Input
      ModeCombinations: []
    - Mode 0: Name: T MOT, Symbol: pwr, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: SupportFunctionalMapping20 Absolute
        Raw Min:    -100, Max:     100
        Pct Min:    -100, Max:     100 (pass-through)
        SI  Min:    -100, Max:     100 (pass-through)
    - Mode 1: Name: ONSEC, Symbol: sec, Capability: Input
      - DataSet: 1x Int32, TotalFigures: 4, Decimals: 0
        Input Mapping: Relative
        Raw Min:       0, Max:       1
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:       1 (pass-through)
````
# TechnicLargeLinearMotor

LEGO Technic smaller default motor.

**Type**: External Motor

**Status**: Pending Issues

## Modes

### Mode 0 - POWER

The percentage of maximum power applied to the motor.

**Direction**: Output

**DataType**: SByte, -100 (CCW) to 100 (CW), special values 0 (floating) and -127 (breaking)

**Notes**
- Setting POWER to 0 or -127 stops the motor

### Mode 1 - SPEED

The percentage of maximum speed currently applied to the motor 

**Direction**: Input | Output

**DataType**:  SByte, -100 (CCW) to 100 (CW), special values 0 (hold position)

**Notes**
- Setting SPEED to 0 holds the position
- For Floating or braking exits StartPower can be used instead.

### Mode 2 - POS

The amount of degrees moved since the motor was started or reset to zero

**Direction**: Input | Output

**DataType**: Int32 up to 10_000 degrees.

**Notes**
- The function Goto(Absolute)Position command refers to this position.

### Mode 3 - APOS

The amount of degrees from an unmarked zero point.

**Direction**: Input | Output

**DataType**: Int16 -360 to 360.

**Notes**
- The function Goto(Absolute)Position command DOEST NOT refers to this position.

## Known Related Commands

- StartPower & StartPower2 (with two motors on a single virtual port)
- StartSpeed & StartSpeed2
- StartSpeedForTime & StartSpeedForTime2
- StartSpeedForDegrees & StartSpeedForDegrees2 (the 2x `degrees` are split between the two motors according to their speed)
- GotoPosition & GotoPosition2
- SetZero (resets the POS mode)

## Open Questions

- How exactly CALIB works
- How exactly LOAD works (most likely how heavy utilized)

## Resources

- TODO

## Port and Port Mode Information

### TechnicMediumHub / Software 0.0.0.1000 / Hardware 0.0.0.1000

Binary Export

````
0B-00-43-00-01-0F-06-1E-00-1F-00
07-00-43-00-02-0E-00
11-00-44-00-00-00-50-4F-57-45-52-00-00-00-00-00-00
0E-00-44-00-00-01-00-00-C8-C2-00-00-C8-42
0E-00-44-00-00-02-00-00-C8-C2-00-00-C8-42
0E-00-44-00-00-03-00-00-C8-C2-00-00-C8-42
0A-00-44-00-00-04-50-43-54-00
08-00-44-00-00-05-00-10
0A-00-44-00-00-80-01-00-01-00
11-00-44-00-01-00-53-50-45-45-44-00-00-00-00-00-00
0E-00-44-00-01-01-00-00-C8-C2-00-00-C8-42
0E-00-44-00-01-02-00-00-C8-C2-00-00-C8-42
0E-00-44-00-01-03-00-00-C8-C2-00-00-C8-42
0A-00-44-00-01-04-50-43-54-00
08-00-44-00-01-05-10-10
0A-00-44-00-01-80-01-00-04-00
11-00-44-00-02-00-50-4F-53-00-00-00-00-00-00-00-00
0E-00-44-00-02-01-00-00-B4-C3-00-00-B4-43
0E-00-44-00-02-02-00-00-C8-C2-00-00-C8-42
0E-00-44-00-02-03-00-00-B4-C3-00-00-B4-43
0A-00-44-00-02-04-44-45-47-00
08-00-44-00-02-05-08-08
0A-00-44-00-02-80-01-02-04-00
11-00-44-00-03-00-41-50-4F-53-00-00-00-00-00-00-00
0E-00-44-00-03-01-00-00-B4-C3-00-00-B4-43
0E-00-44-00-03-02-00-00-C8-C2-00-00-C8-42
0E-00-44-00-03-03-00-00-B4-C3-00-00-B4-43
0A-00-44-00-03-04-44-45-47-00
08-00-44-00-03-05-08-08
0A-00-44-00-03-80-01-01-03-00
11-00-44-00-04-00-4C-4F-41-44-00-00-00-00-00-00-00
0E-00-44-00-04-01-00-00-00-00-00-00-FE-42
0E-00-44-00-04-02-00-00-00-00-00-00-C8-42
0E-00-44-00-04-03-00-00-00-00-00-00-FE-42
0A-00-44-00-04-04-50-43-54-00
08-00-44-00-04-05-08-08
0A-00-44-00-04-80-01-00-01-00
11-00-44-00-05-00-43-41-4C-49-42-00-00-00-00-00-00
0E-00-44-00-05-01-00-00-00-00-00-00-00-44
0E-00-44-00-05-02-00-00-00-00-00-00-C8-42
0E-00-44-00-05-03-00-00-00-00-00-00-00-44
0A-00-44-00-05-04-52-41-57-00
08-00-44-00-05-05-00-00
0A-00-44-00-05-80-03-01-03-00
````

Human Readable Interpretation

````
  - Port: 0x00 / 0
    - IOTypeId: TechnicLargeLinearMotor / 0x002E / 46
      Revision: SW: 0.0.0.1000, HW: 0.0.0.1000       
      Capabilities: Output Input LogicalCombinable LogicalSynchronizable
      ModeCombinations: [0000000000001110]
    - Mode 0: Name: POWER, Symbol: PCT, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 1, Decimals: 0
        Output Mapping: Absolute
        Raw Min:    -100, Max:     100
        Pct Min:    -100, Max:     100 (pass-through)
        SI  Min:    -100, Max:     100 (pass-through)
    - Mode 1: Name: SPEED, Symbol: PCT, Capability: Input Output
      - DataSet: 1x SByte, TotalFigures: 4, Decimals: 0
        Input Mapping: Absolute
        Output Mapping: Absolute
        Raw Min:    -100, Max:     100
        Pct Min:    -100, Max:     100 (pass-through)
        SI  Min:    -100, Max:     100 (pass-through)
    - Mode 2: Name: POS, Symbol: DEG, Capability: Input Output
      - DataSet: 1x Int32, TotalFigures: 4, Decimals: 0
        Input Mapping: Relative
        Output Mapping: Relative
        Raw Min:    -360, Max:     360
        Pct Min:    -100, Max:     100 (scaling)
        SI  Min:    -360, Max:     360 (pass-through)
    - Mode 3: Name: APOS, Symbol: DEG, Capability: Input Output
      - DataSet: 1x Int16, TotalFigures: 3, Decimals: 0
        Input Mapping: Relative
        Output Mapping: Relative
        Raw Min:    -360, Max:     360
        Pct Min:    -100, Max:     100 (scaling)
        SI  Min:    -360, Max:     360 (pass-through)
    - Mode 4: Name: LOAD, Symbol: PCT, Capability: Input Output
      - DataSet: 1x SByte, TotalFigures: 1, Decimals: 0
        Input Mapping: Relative
        Output Mapping: Relative
        Raw Min:       0, Max:     127
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     127 (pass-through)
    - Mode 5: Name: CALIB, Symbol: RAW, Capability:
      - DataSet: 3x Int16, TotalFigures: 3, Decimals: 0
        Raw Min:       0, Max:     512
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:     512 (pass-through)
````
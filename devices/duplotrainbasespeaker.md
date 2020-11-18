# DuploTrainBaseSpeaker

Speaker integrated in the DuploTrainBase.

**Type**: Hub Device

**Status**: Pending Issues

## Modes

### 🕵️‍♀️ Mode 0 - Tone

Play a tone?

**Direction**: Output

**DataType**: TODO

**Notes**
- TODO

### Mode 1 - Sound

When invoked, allows to play a set of pre-defined sounds on the device. 

**Direction**: Output

**DataType**: sbyte addressing a dictionary of predefined sounds which can be played. See supplementary documentation below.

### 🕵️‍♀️ Mode 2 - UI Sound

Play a tone?

**Direction**: Output

**DataType**: sbyte

**Notes**
- TODO

## Known Related Commands

- WriteDirectModeData on mode 1 with a given value below.

## Supplementary Definitions

### Predefined Sounds

| Idx | Sound |
| --- | --- |
| 3 | Brake |
| 5 | StationDeparture |
| 7 | WaterRefill |
| 9 | Horn |
| 10 | Steam |

## Open Questions

- How to operate mode 0 and mode 2?

## Resources

- Dictionary from [nathankellenicki/node-poweredup](https://github.com/nathankellenicki/node-poweredup)

## Port and Port Mode Information

### DuploTrainBaseHub / Software 0.0.0.1 / Hardware 0.0.0.1

Binary Export

````
06-00-01-0B-06-20
0F-00-04-01-01-2A-00-01-00-00-00-01-00-00-00
0B-00-43-01-01-01-03-00-00-07-00
05-00-43-01-02
11-00-44-01-00-00-54-4F-4E-45-00-00-00-00-00-00-00
0E-00-44-01-00-01-00-00-00-00-00-00-20-41
0E-00-44-01-00-02-00-00-00-00-00-00-C8-42
0E-00-44-01-00-03-00-00-00-00-00-00-20-41
0A-00-44-01-00-04-69-64-78-00
08-00-44-01-00-05-00-04
0A-00-44-01-00-80-01-00-03-00
11-00-44-01-01-00-53-4F-55-4E-44-00-00-00-00-00-00
0E-00-44-01-01-01-00-00-00-00-00-00-20-41
0E-00-44-01-01-02-00-00-00-00-00-00-C8-42
0E-00-44-01-01-03-00-00-00-00-00-00-20-41
0A-00-44-01-01-04-69-64-78-00
08-00-44-01-01-05-00-44
0A-00-44-01-01-80-01-00-03-00
11-00-44-01-02-00-55-49-20-53-4E-44-00-00-00-00-00
0E-00-44-01-02-01-00-00-00-00-00-00-20-41
0E-00-44-01-02-02-00-00-00-00-00-00-C8-42
0E-00-44-01-02-03-00-00-00-00-00-00-20-41
0A-00-44-01-02-04-69-64-78-00
08-00-44-01-02-05-00-04
0A-00-44-01-02-80-01-00-03-00
````

Human Readable Interpretation

````
  - Port: 0x01 / 1
    - IOTypeId: DuploTrainBaseSpeaker / 0x002A / 42
      Revision: SW: 0.0.0.1, HW: 0.0.0.1
      Capabilities: Output
      ModeCombinations: []
    - Mode 0: Name: TONE, Symbol: idx, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 1: Name: SOUND, Symbol: idx, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: SupportFunctionalMapping20 Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
    - Mode 2: Name: UI SND, Symbol: idx, Capability: Output
      - DataSet: 1x SByte, TotalFigures: 3, Decimals: 0
        Output Mapping: Discrete
        Raw Min:       0, Max:      10
        Pct Min:       0, Max:     100 (scaling)
        SI  Min:       0, Max:      10 (pass-through)
````
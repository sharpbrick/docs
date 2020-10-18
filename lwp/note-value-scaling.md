## LWP Note: Value Scaling

### Removing the Mind Block

The LEGO Wireless protocol exposes the following properties in regards of a value

- Raw Min / Max
- Pct Min / Max
- SI Min / Max

The Value itself has a data type (SByte (signed 8 bit integer), Int16 (signed 16 bit integer), Int32 (signed 32 bit integer), Single (4-byte IEEE754 floating point)).

The following **mental adjustments** is necessary: Raw Min/Max **are not (necessarily) the upper and lower limit** of the value range. Neither is this true for Pct Min/Max and SI Min/Max.

### Value Scaling / Shifting

Instead, the 6 boundaries are used to establish scaling/shifting factor on the provided value for each, the SI and Percentage range. The following formula is applicable for all Powered UP devices verified against the approach so far w/o exception.

````csharp
var positionInRawRange = (value - rawMin) / (rawMax - rawMin);

return (positionInRawRange * (max - min)) + min;
````

### Pass Through Original Value

Applied in many devices (e.g. which return discrete value).

- Raw Min / Max: 10 / 10
- SI Min / Max: 10 / 10

**Result**: The original value passes through the formula and remains unchanged. The boundaries invalidate themselves.

# SPWN Beta Test

As a part of the beta testing team I decided to make my first SPWN project a binary calculator library.

## Usage

see [the runner](/runner.spwn).

## Functions from @binaryCalculator

A list of all functions and how to use them.

### ::new

The class constructor.

```swift
@binaryCalculator::new(bits: @number, x: @number, y: @number);
```

- bits: The amount of bits in the binary number
- x: The base X position of the bits
- y: The Y position of the bits

### binaryToDecimal

A conversion method to turn the bits into a decimal number which is stored in the target.

```swift
binaryCalculator.binaryToDecimal(target: @counter);
```

- target: The target counter storage

### decimalToBinary

A conversion method to convert the source into binary which is stored in the provided bits.

```swift
binaryCalculator.decimalToBinary(source: @counter);
```

- source: The counter source

### prettyDecimalToBinary

A slower but more interesting and clear version of [decimalToBinary](#decimalToBinary) showing how the number iterates through its division cycles. This uses less logic so it can handle larger numbers without exceeding the group limit.

```swift
binaryCalculator.prettyDecimalToBinary(source: @counter);
```

- source: The counter source

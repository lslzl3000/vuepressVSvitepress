[@dev/core](../README.md) / [Exports](../modules.md) / ITimerData

# Interface: ITimerDataT

An interface defining the data sent by the timer

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [completeRate](ITimerData.md#completerate)
- [currentTime](ITimerData.md#currenttime)
- [deltaTime](ITimerData.md#deltatime)
- [payload](ITimerData.md#payload)
- [startTime](ITimerData.md#starttime)

## Properties

### completeRate

• **completeRate**: `number`

How much is completed, in [0.0...1.0].
Note that this CAN be higher than 1 due to the fact that we don't actually measure time but delta between observable calls

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:66

___

### currentTime

• **currentTime**: `number`

Time now

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:57

___

### deltaTime

• **deltaTime**: `number`

Time passed since started

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:61

___

### payload

• **payload**: `T`

What the registered observable sent in the last count

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:70

___

### startTime

• **startTime**: `number`

When did it start

#### Defined in

https://github.com/babylon.js/core/src/Misc/timer.ts:53

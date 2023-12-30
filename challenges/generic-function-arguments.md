# Generic Function Arguments

## Challenge

https://typehero.dev/challenge/generic-function-arguments

## Answer

```ts
const identity = <T,>(value: T) => value;

type MapFN<T, K> = (value: T, index: number, array: T[]) => K;
const mapArray = <T, K>(arr: T[], fn: MapFN<T, K>) => arr.map(fn);
```
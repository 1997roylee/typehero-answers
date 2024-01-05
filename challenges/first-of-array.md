# First of Array

## Challenge

https://typehero.dev/challenge/first-of-array

## Answer

```ts
type First<T extends unknown[]> = T["length"] extends 0 ? never : T[0];
```
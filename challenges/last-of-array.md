# Last of Array

## Challenge

https://typehero.dev/challenge/last-of-array

## Answer

```ts
type Last<T extends any[]> = T extends [...any[], infer U] ? U : never;
// type Last<T extends any[]> = [0, ...T][T["length"]];
```
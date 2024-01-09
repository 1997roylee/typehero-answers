# Push

## Challenge

https://typehero.dev/challenge/push

## Answer

```ts
type Push<T, U> = T extends unknown[]?[...T, U]: never
```
# Unshift

## Challenge

https://typehero.dev/challenge/unshift

## Answer

```ts
type Unshift<T extends unknown[], U> = [U, ...T];
```
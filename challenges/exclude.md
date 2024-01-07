# Exclude

## Challenge

https://typehero.dev/challenge/exclude

## Answer

```ts
type MyExclude<T, U> = T extends U ? never: T
```
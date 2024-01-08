# Concat

## Challenge

https://typehero.dev/challenge/concat/submissions/177255?success=true

## Answer

```ts
type Concat<T extends readonly unknown[], U extends readonly unknown[]> = [...T, ...U];
```
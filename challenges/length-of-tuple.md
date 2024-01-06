# Length of Tuple

## Challenge

https://typehero.dev/challenge/length-of-tuple

## Answer

```ts
type Length<T extends readonly string[]> = T['length']
```
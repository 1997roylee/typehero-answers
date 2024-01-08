# If

## Challenge

https://typehero.dev/challenge/if/submissions/177257?success=true

## Answer

```ts
type If<C extends boolean, T, F> = C extends true ? T : F;
```
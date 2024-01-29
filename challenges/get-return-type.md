# Get Return Type

## Challenge

https://typehero.dev/challenge/get-return-type

## Answer

```ts
type MyReturnType<T> = T extends (...args: any) => infer Return ? Return : never;
```
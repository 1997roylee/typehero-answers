# Awaited

## Challenge

https://typehero.dev/challenge/awaited

## Answer

```ts
type PromiseCallback = { then: (onfulfilled: (arg: number) => any) => any };
type MyAwaited<T extends Promise<unknown> | PromiseCallback> = Awaited<T>;
```
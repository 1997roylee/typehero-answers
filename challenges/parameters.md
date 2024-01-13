# Parameters

## Challenge

https://typehero.dev/challenge/parameters

## Answer

```ts
type MyParameters<T extends (...args: any[]) => any> = T extends (...args: infer Args) => any
	? Args
	: never;
```
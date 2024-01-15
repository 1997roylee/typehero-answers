# The `Pick` builtin

## Challenge

https://typehero.dev/challenge/pick

## Answer

```ts
type MyPick<T, K extends keyof T> = {
	[Key in K]: T[Key];
};
```
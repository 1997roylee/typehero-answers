# Omit

## Challenge

https://typehero.dev/challenge/omit

## Answer

```ts
type MyOmit<T extends {}, K extends keyof T> = {
	[Key in keyof T as Key extends K ? never : Key]: T[Key];
};
```
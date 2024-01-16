# All

## Challenge

https://typehero.dev/challenge/all

## Answer

```ts
type IsEqual<A, B> = (<T>() => T extends A ? 1 : 2) extends <T>() => T extends B ? 1 : 2
	? true
	: false;

type All<T extends unknown[], U> = IsEqual<
	{
		[K in keyof T]: IsEqual<T[K], U>;
	}[number],
	true
>;
```
# Tuple to Object

## Challenge

https://typehero.dev/challenge/tuple-to-object

## Answer

```ts
type TupleToObject<T extends readonly (string | number | symbol)[]> = {
	[K in T[number]]: K;
};
```
# Absolute

## Challenge

https://typehero.dev/challenge/absolute/solutions/381

## Answer

```ts
type Absolute<T extends number | string | bigint> = `${T}` extends `-${infer Number}`
	? `${Number}`
	: `${T}`;
```
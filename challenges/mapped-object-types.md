# Mapped Object Types

## Challenge

https://typehero.dev/challenge/mapped-object-types

## Answer

```ts
type MovieInfoByGenre<T> = {
	[K in keyof T]: {
		name: T[K] | string;
		year: number;
		director: string;
	};
};
```
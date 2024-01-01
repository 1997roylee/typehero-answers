# Generic Type Constraints

## Challenge

https://typehero.dev/challenge/generic-type-constraints

## Answer

```ts
type AllowString<T extends string> = T;
type AllowNumber<T extends number> = T;

type CreateLogger<T extends (arg0: number) => void> = {
	log: T;
	exit: () => void;
};
```
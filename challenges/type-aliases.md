# Type Aliases

## Challenge

https://typehero.dev/challenge/type-aliases

## Answer

```ts
type Name = string;
type Year = number;
type Count = number;
type IsOperational = boolean;
type Kilograms = number;

type Payload = {
	name: Name;
	mass: Kilograms;
};
```
# [Tutorial Title]

## Challenge

https://typehero.dev/challenge/readonly

## Thought

Loop object keys and assign readonly to each property.

## Answer

```ts
type MyReadonly<T> = {
	readonly [P in keyof T]: T[P];
};
```
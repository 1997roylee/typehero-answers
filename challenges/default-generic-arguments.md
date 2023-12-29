# Default Generic Arguments

## Challenge

https://typehero.dev/challenge/default-generic-arguments

## Answer

```ts
type ApiRequest<TData, TMethod = "GET"> = {
	data: TData;
	method: TMethod;
};

type TSConfig<TConfig extends { strict: boolean } = { strict: true }> = TConfig;
```
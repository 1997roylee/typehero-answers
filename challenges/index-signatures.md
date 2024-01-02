# Index Signatures

## Challenge

https://typehero.dev/challenge/index-signatures

## Answer

```ts
type GroceryList = {
	[item: string]: number;
};

type InappropriateActionBySituation = {
	[action: string]: string[];
};

type CharactersById = {
	[id: number]: {
		id: number;
		name: string;
		status: string;
		species: string;
	};
};
```
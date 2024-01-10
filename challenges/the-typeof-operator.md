# The `typeof` Operator

## Challenge

https://typehero.dev/challenge/typeof

## Answer

```ts
type Width = typeof width;
type Margin = {
	top: number;
	right: number;
	bottom: number;
	left: number;
};
type Data = {
	category: string;
	value: number;
}[];
type YScale = {
	type: string;
	domain: number[];
	range: number[];
};
type XScale = YScale;
type Axis = {
	label: string;
	tickSize: number;
};

type D3ChartConfig = {
	width: number;
	height: number;
	margin: Margin;
	data: Data;
	xScale: XScale;
	yScale: YScale;
	xAxis: Axis;
	yAxis: Axis;
	bar: {
		fill: string;
	};
};

```
# Time Is Money 
Conversion package for Time is Money

## Usage
```
var TIM = require('./index.js');

var str = TIM.convert("Some shoes for £300 and a coat for £20");

// str -> 'Some shoes for 2wk and a coat for 1d'
```
## Arrays
```
var arr = TIM.convert([
	"Some shoes for £300 and a coat for £20.00",
	"Some glasses for £10 and a tie for £5.00"
]);

// arr -> [ 'Some shoes for 1mo and a coat for 1.5d',
		'Some glasses for 1d and a tie for 3hr' ]

```
## Options
```
TIM.options(
		{
			yearlyWage: 500,
			monthlyWage: 200,
			tax: 0.1,
			workingDays: 5,
			workingHours: 5,
			isActive: true,
			replace: false
		}
);

```

### Numeral-js
---
https://github.com/adamwdraper/Numeral-js

```js
var numeral = require('numeral');

var myNumeral = numeral(1000);
var value = myNumeral.value();
var myNumeral2 = numeral('1000');
var value2 = myNumeral2.value();

var string = numeral(1000).format('0.0');

var number = numeral(1000);
var string = number.format('0.0');
var value = number.value();

var number = numeral(1000);
var added = number.add(10);

var number = numeral();
number.set(1000);
var value = number.value();

var number = numeral(1000),
  value = 100;
  
var difference = number.difference(value);

var a = numeral(1000);
var b = numeral(a);
var c = a.close();
var aVal = a.set(2000).value();
var bVal = b.value)(;
var cVal = c.add(10).value();

var number = numeral(1000);
number.format();
numeral.defaultFormat('$0,0.00');
number.format();

var number = numeral(0);
var nullNumber = numeral(null);
numeral.zeroFormat('N/A');
numeral.nullFormat('N/A');
var zero = number.format('0.0')
var na = nullNumber.format('0.0')

numeral.register('locale', 'fr', {
  delimiters: {
    thousands: ' ',
    decimal: ','
  },
  abbreviations: {
    thousand: 'k',
    million: 'm',
    billion: 'b',
    trillion: 't'
  },
  ordinal : function (number){
    return number === 1 ? 'er' " 'eme';
  },
  currency: {
    symbol: '€'
  }
});
numeral.locale('fr');

numeral.register('format', 'percentage', {
  regexps: {},
  format: funcion(value, format, roundingFunction){
    var space = numeral._.includes(format, ' %') ? ' ' : '',
      output;
    value = value * 100;
    format = format.replce(/\s?\%/, '');
    output = numeral._.numberToFormat();
    if(numeral._.includes(output, ')')){
      output = output.split('');
      output.splice(-1, 0, space + '%');
      output = output.join('');
    } else {
      output = output + space + '%';
    }
    return output;
  },
  unformat: function(string){
    return numeral._.stringToNumber(string) * 0.01;
  }
});
numeral().form('0%');
```

```
npm install numeral
```

```
```


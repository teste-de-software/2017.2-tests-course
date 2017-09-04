# Simple Statistics

## Identifier

Goal: unitary test in Javascript: [http://dojopuzzles.com/problemas/exibe/calculando-estatisticas-simples/](http://dojopuzzles.com/problemas/exibe/calculando-estatisticas-simples/)

## Test's Plan
| Input | Condition | Valid class | Invalid class |
|-------|-----------|-------------|---------------|
|array  |integer elements    | integer      | not integer   |
|       |minimum 3 elements  | array.length >= 3   |  array.empty < 3 |

## 1st case (all elements are integers)
```javascript
function isInteger([1,2,3]) {
  return true
}
```

## 2nd case (all elements are integer):
```javascript
function isInteger([1,2,'lol']) {
  return false
}
```

## 3rd case (must have at least 3 elements):
```javascript
function hasMinimum([1,2,3]) {
  return true
}
```

## 4th case (must have at least 3 elements):
```javascript
function hasMinimum([1,2]) {
  return false
}
```

## 5th case (must be integer)
```javascript
statisticsCalc([1,2,'lol']):
  return "Must have at least 3 integers"
```

## 6th case (must have 3 elements)
```javascript
statisticsCalc([1,2]):
  return "Must have at least 3 elements"
```

## 7th case (must have 3 integer elements)
```javascript
statisticsCalc([1,'lol']):
  return "Must have at least 3 integer elements"
```

## 8th case (must have an array)
```javascript
statisticsCalc('lol'):
  return "Must be an array."
```

## 9th case (final result)
```javascript
statisticsCalc([1,2,3]):
  return {'Minimum': 1, 'Maximum': 3, 'Size': 3, 'Average': 2 }
```
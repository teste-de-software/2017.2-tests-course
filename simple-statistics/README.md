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
statisticsCalc([1,-2,3]):
  return true
```

## 2nd case (all elements are integer):
```javascript
statisticsCalc(['lol']):
  // throws expection
```

## 3rd case (must have at least 3 elements):
```javascript
statisticsCalc([1,2,3]):
  return true
```

## 4th case (must have at least 3 elements):
```javascript
statisticsCalc([1,2]):
  // throws expection
```

## 5th case (final result)
```javascript
statisticsCalc([1,2,3]):
  return {'Minimum': 1, 'Maximum': 3, 'Size': 3, 'Media': 2]
```

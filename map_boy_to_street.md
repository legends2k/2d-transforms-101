## Map Boy To Kids Room

* R135
```
[ [ -0.707106781187, 0.707106781187,  0 ]
  [ -0.707106781187, -0.707106781187, 0 ]
  [        0,               0,        1 ] ]
```
* T4,2
```
[ [ 1, 0, 0 ]
  [ 0, 1, 0 ]
  [ 4, 2, 1 ] ]
```

## Map Kids Room To House
* R−90
```
[ [ 0, -1, 0 ]
  [ 1, 0,  0 ]
  [ 0, 0,  1 ] ]
```
* S½,½
```
[ [ 0.5,  0,  0 ]
  [  0,  0.5, 0 ]
  [  0,   0,  1 ] ]
```
* T2,4
```
[ [ 1, 0, 0 ]
  [ 0, 1, 0 ]
  [ 2, 4, 1 ] ]
```

## Map House To Street
* T0,−6
```
[ [ 1,  0,  0 ]
  [ 0,  1,  0 ]
  [ 0, -6, 1 ] ]
```
* S1,−1
```
[ [ 1, 0,  0 ]
  [ 0, -1, 0 ]
  [ 0, 0,  1 ] ]
```
* S⅔,⅔
```
[ [ 0.666666666667,        0,        0 ]
  [       0,         0.666666666667, 0 ]
  [       0,               0,        1 ] ]
```

## Result

```
Mb→s = Ls→b = Lk→b Lh→k Ls→h
      = (R135 T4,2) (R−90 S½,½ T2,4) (T0,−6 S1,−1 S⅔,⅔)
      = [ [ 0.2357,  -0.2357, 0 ]
          [ -0.2357, -0.2357, 0 ]
          [    2,    2.6667,  1 ] ]
```

This follows [row-vector](http://en.wikipedia.org/wiki/Row_vector) convention. Transpose and reverse the order of multiplication to get the same result in [column-vector](http://en.wikipedia.org/wiki/Column_vector) convention.

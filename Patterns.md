<div class="cell code" data-execution_count="17">

```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(r):
        print('*', end='')
    print()
```

<div class="output stream stdout">

    *****
    *****
    *****
    *****
    *****

</div>

</div>

<div class="cell code" data-execution_count="3">

```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(i+1):
        print('*', end='')
    print()
```

<div class="output stream stdout">

    *
    **
    ***
    ****
    *****

</div>

</div>

<div class="cell code" data-execution_count="60">

```python
r = int(input('enter rows :'))
for i in range(r, 0, -1):
    for j in range(i):
        print('*', end='')
    print()
```

<div class="output stream stdout">

    *****
    ****
    ***
    **
    *

</div>

</div>

<div class="cell code" data-execution_count="13">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(r, 0, -1):
        print(' ', end='')
    r -= 1
    for j in range(i):
        print('*', end='')
    print()
```

<div class="output stream stdout">

```
     *
    **
   ***
  ****
 *****
```

</div>

</div>

<div class="cell code" data-execution_count="11">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(1, i):
        print(' ', end='')
    for j in range(r, 0, -1):
        print("*", end='')
    r -= 1
    print()
```

<div class="output stream stdout">

    *****
     ****
      ***
       **
        *

</div>

</div>

<div class="cell code" data-execution_count="67">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(r, 0, -1):
        print(' ', end='')
    r -= 1
    for j in range(1, i*2):
        print('*', end='')
    print()
```

<div class="output stream stdout">

```
     *
    ***
   *****
  *******
 *********
```

</div>

</div>

<div class="cell code" data-execution_count="65">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(1, i):
        print(' ', end='')
    for j in range(r*2, 1, -1):
        print("*", end='')
    r -= 1
    print()
```

<div class="output stream stdout">

    *********
     *******
      *****
       ***
        *

</div>

</div>

<div class="cell code" data-execution_count="49">

```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(i+1):
        print('*', end=' ')
    print()
```

<div class="output stream stdout">

```
*
* *
* * *
* * * *
* * * * *
```

</div>

</div>

<div class="cell code" data-execution_count="50">

```python
r = int(input('enter rows :'))
for i in range(r, 0, -1):
    for j in range(i):
        print('*', end=' ')
    print()
```

<div class="output stream stdout">

```
* * * * *
* * * *
* * *
* *
*
```

</div>

</div>

<div class="cell code" data-execution_count="55">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(r*2, 0, -1):
        print(' ', end='')
    r -= 1
    for j in range(i):
        print('*', end=' ')
    print()
```

<div class="output stream stdout">

```
          *
        * *
      * * *
    * * * *
  * * * * *
```

</div>

</div>

<div class="cell code" data-execution_count="58">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(1, i*2):
        print(' ', end='')
    for j in range(r, 0, -1):
        print("*", end=' ')
    r -= 1
    print()
```

<div class="output stream stdout">

```
 * * * * *
   * * * *
     * * *
       * *
         *
```

</div>

</div>

<div class="cell code" data-execution_count="63">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(r, 0, -1):
        print(' ', end='')
    r -= 1
    for j in range(i):
        print('*', end=' ')
    print()
```

<div class="output stream stdout">

```
     *
    * *
   * * *
  * * * *
 * * * * *
```

</div>

</div>

<div class="cell code" data-execution_count="61">

```python
r = int(input('enter rows :'))
for i in range(1, r+1):
    for k in range(1, i):
        print(' ', end='')
    for j in range(r, 0, -1):
        print("*", end=' ')
    r -= 1
    print()
```

<div class="output stream stdout">

```
* * * * *
 * * * *
  * * *
   * *
    *
```

</div>

</div>

<div class="cell code" data-execution_count="1">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        print(i, end='')
    print()
```

<div class="output stream stdout">

    11111
    22222
    33333
    44444
    55555

</div>

</div>

<div class="cell code" data-execution_count="31">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        print(j, end='')
    print()
```

<div class="output stream stdout">

    12345
    12345
    12345
    12345
    12345

</div>

</div>

<div class="cell code" data-execution_count="29">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, i+1):
        print(j, end='')
    print()
```

<div class="output stream stdout">

    1
    12
    123
    1234
    12345

</div>

</div>

<div class="cell code" data-execution_count="43">

```python
r = 5
x = r
for i in range(1, r+1):
    for k in range(x, 0, -1):
        print(' ', end='')
    x -= 1
    for j in range(1, i*2):
        print(j, end='')
    print()
```

<div class="output stream stdout">

```
     1
    123
   12345
  1234567
 123456789
```

</div>

</div>

<div class="cell code" data-execution_count="4">

```python
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        print(chr(c), end='')
    print()
    c += 1
```

<div class="output stream stdout">

    A
    BB
    CCC
    DDDD
    EEEEE

</div>

</div>

<div class="cell code" data-execution_count="66">

```python
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        print(chr(c), end='')
        c += 1
    print()
```

<div class="output stream stdout">

    A
    BC
    DEF
    GHIJ
    KLMNO

</div>

</div>

<div class="cell code" data-execution_count="16">

```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(r):
        if (i == 0) or (i == r-1) or (j == 0) or (j == r-1):
            print('*', end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    *****
    *   *
    *   *
    *   *
    *****

</div>

</div>

<div class="cell code" data-execution_count="20">

```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(i+1):
        if (i == 0) or (i == r-1) or (j == 0) or (j == i):
            print('*', end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    *
    **
    * *
    *  *
    *****

</div>

</div>

<div class="cell code" data-execution_count="23">

```python
r = int(input('enter rows :'))
for i in range(r, 0, -1):
    for j in range(i):
        if (i == r) or (i == 1) or (j == 0) or (j == i-1):
            print('*', end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    *****
    *  *
    * *
    **
    *

</div>

</div>

<div class="cell code" data-execution_count="33">

```python
r = int(input('enter rows :'))
z = r
for i in range(1, r+1):
    for k in range(z, 0, -1):
        print(' ', end='')
    for j in range(i):
        if (i == r) or (i == 0) or (j == 0) or (j == i-1):
            print('*', end='')
        else:
            print(' ', end='')
    z -= 1
    print()
```

<div class="output stream stdout">

```
     *
    **
   * *
  *  *
 *****
```

</div>

</div>

<div class="cell code" data-execution_count="40">

```python
r = int(input('enter rows :'))
z = r
for i in range(1, r+1):
    for k in range(1, i):
        print(' ', end='')
    for j in range(z, 0, -1):
        if (i == r) or (i == 1) or (j == z) or (j == 1):
            print('*', end='')
        else:
            print(' ', end='')
    z -= 1
    print()
```

<div class="output stream stdout">

    *****
     *  *
      * *
       **
        *

</div>

</div>

<div class="cell code" data-execution_count="17">

```python
r = int(input('enter rows :'))
z = r
for i in range(1, r+1):
    for k in range(z, 0, -1):
        print(' ', end='')
    z -= 1
    for j in range(1, i*2):
        if (i == r) or (i == 1) or (j == 1) or (j == (i*2)-1):
            print('*', end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

```
     *
    * *
   *   *
  *     *
 *********
```

</div>

</div>

<div class="cell code" data-execution_count="16">

```python
r = int(input('enter rows :'))
x = r
for i in range(1, r+1):
    for k in range(1, i):
        print(' ', end='')
    for j in range(x*2, 1, -1):
        if (i == r) or (i == 1) or (j == 2) or (j == x*2):
            print('*', end='')
        else:
            print(' ', end='')
    x -= 1
    print()
```

<div class="output stream stdout">

    *********
     *     *
      *   *
       * *
        *

</div>

</div>

<div class="cell code" data-execution_count="32">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        if(i == 1) or (i == r) or (j == 1) or (j == r):
            print(j, end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    12345
    1   5
    1   5
    1   5
    12345

</div>

</div>

<div class="cell code" data-execution_count="18">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        if(i == 1) or (i == r) or (j == 1) or (j == r):
            print(i, end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    11111
    2   2
    3   3
    4   4
    55555

</div>

</div>

<div class="cell code" data-execution_count="36">

```python
r = 5
for i in range(1, r+1):
    for j in range(1, i+1):
        if(i == 1) or (i == r) or (j == 1) or (j == i):
            print(j, end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

    1
    12
    1 3
    1  4
    12345

</div>

</div>

<div class="cell code" data-execution_count="20">

```python
r = 5
x = r
for i in range(1, r+1):
    for k in range(x, 0, -1):
        print(' ', end='')
    x -= 1
    for j in range(1, i*2):
        if(i == 1) or (i == r) or (j == 1) or (j == i*2-1):
            print(j, end='')
        else:
            print(' ', end='')
    print()
```

<div class="output stream stdout">

```
     1
    1 3
   1   5
  1     7
 123456789
```

</div>

</div>

<div class="cell code" data-execution_count="24">

```python
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        if(i == 1) or (i == r) or (j == 0) or (j == i-1):
            print(chr(c), end='')
        else:
            print(' ', end='')
    print()
    c += 1
```

<div class="output stream stdout">

    A
    BB
    C C
    D  D
    EEEEE

</div>

</div>

<div class="cell code" data-execution_count="26">

```python
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        if(i == 1) or (i == r) or (j == 0) or (j == i-1):
            print(chr(c), end='')
        else:
            print(' ', end='')
        c += 1
    print()
```

<div class="output stream stdout">

    A
    BC
    D F
    G  J
    KLMNO

</div>

</div>

# Python Patterns Snippets
There are different types of useful Patterns snippets below
#
### pattern
```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(r):
        print('*', end='')
    print()
```
### output
```
*****
*****
*****
*****
*****
```
#
### pattern
```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(i+1):
        print('*', end='')
    print()
```
### output
```
*
**
***
****
*****
```
#
### pattern
```python
r = int(input('enter rows :'))
for i in range(r, 0, -1):
    for j in range(i):
        print('*', end='')
    print()
```
### output
```
*****
****
***
**
*
```
#
### pattern
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
### output
```
     *
    **
   ***
  ****
 *****
```
#
### pattern
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
### output
```
*****
 ****
  ***
   **
    *
```
#
### pattern
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
### output
```
     *
    ***
   *****
  *******
 *********
```
#
### pattern
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
### output
```
*********
 *******
  *****
   ***
    *
```
#
### pattern
```python
r = int(input('enter rows :'))
for i in range(r):
    for j in range(i+1):
        print('*', end=' ')
    print()
```
### output
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
#
### pattern
```python
r = int(input('enter rows :'))
for i in range(r, 0, -1):
    for j in range(i):
        print('*', end=' ')
    print()
```
### output
```
* * * * * 
* * * * 
* * * 
* * 
* 
```
#
### pattern
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
### output
```
          * 
        * * 
      * * * 
    * * * * 
  * * * * * 
```
#
### pattern
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
### output
```
 * * * * * 
   * * * * 
     * * * 
       * * 
         * 
```
#
### pattern
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
### output
```
     * 
    * * 
   * * * 
  * * * * 
 * * * * * 
```
#
### pattern
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
### output
```
* * * * * 
 * * * * 
  * * * 
   * * 
    *
```
#
### pattern
```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        print(i, end='')
    print()
```
### output
```
11111
22222
33333
44444
55555
```
#
### pattern
```python
r = 5
for i in range(1, r+1):
    for j in range(1, r+1):
        print(j, end='')
    print()
```
### output
```
12345
12345
12345
12345
12345
```
#
### pattern
```python
r = 5
for i in range(1, r+1):
    for j in range(1, i+1):
        print(j, end='')
    print()
```
### output
```
1
12
123
1234
12345
```
#
### pattern
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
### output
```
     1
    123
   12345
  1234567
 123456789
```
#
### pattern
```python
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        print(chr(c), end='')
    print()
    c += 1
```
### output
```
A
BB
CCC
DDDD
EEEEE
```
#

### pyramid
```python 
c = 65
r = 5
for i in range(1, r+1):
    for j in range(i):
        print(chr(c), end='')
        c += 1
    print()
```
### output 
```
A
BC
DEF
GHIJ
KLMNO
```
#

# Hollow  Pyramids 
### Pattern
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
### output 
```
*****
*   *
*   *
*   *
*****
```
#


### pattern 
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
### output 
```
*
**
* *
*  *
*****
```
#


### pattern 
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
### output 
```
*****
*  *
* *
**
*
```
#


### pattern 
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
### output 
```
     *
    **
   * *
  *  *
 *****
```
#


### pattern 
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
### output 
```
*****
 *  *
  * *
   **
    *
```
#


### pattern 
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
### output 
```
     *
    * *
   *   *
  *     *
 *********
```
#


### pattern 
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
### output 
```
*********
 *     *
  *   *
   * *
    *
```
#


### pattern 
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
### output 
```
12345
1   5
1   5
1   5
12345
```
#


### pattern 
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
### output 
```
11111
2   2
3   3
4   4
55555
```
#


### pattern 
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
### output 
```
1
12
1 3
1  4
12345
```
#

### pattern
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

### output
```
     1
    1 3
   1   5
  1     7
 123456789
```
#
### pattern
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

### output
```
A
BB
C C
D  D
EEEEE
```
#
### pattern
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

### output
```
A
BC
D F
G  J
KLMNO
```
#

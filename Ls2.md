

```python
z = 1<100
print(z)
```

    True



```python
z = True
```


```python
sport = 'football'
print(sport)
```

    football



```python
letter = sport[1]
letter
```




    'o'




```python
letter = sport[2:4]
letter
```




    'ot'




```python
fam_height = ['father',1.78,'mother',1.68,'son',1.8,'daughter',1.65]
fam_height
```




    ['father', 1.78, 'mother', 1.68, 'son', 1.8, 'daughter', 1.65]




```python
mix = ['a',1,['b',4.2]]
mix
```




    ['a', 1, ['b', 4.2]]




```python
fam_height[1]
```




    1.78




```python
fam_height[7]
```




    1.65




```python
fam_height[-1]
```




    1.65




```python
fam_height[-3]
```




    1.8




```python
fam_height[-4]
```




    'son'




```python
fam_height[2:4]
```




    ['mother', 1.68]




```python
fam_height[:4]
```




    ['father', 1.78, 'mother', 1.68]




```python
fam_height[4:]
```




    ['son', 1.8, 'daughter', 1.65]




```python
fam_height[:]
```




    ['father', 1.78, 'mother', 1.68, 'son', 1.8, 'daughter', 1.65]




```python
x = [["a","b","c"],
    ["d","e","f"],
    ["g","h","i"]]
```


```python
type(x)
```




    list




```python
x[0]
```




    ['a', 'b', 'c']




```python
x[1]
```




    ['d', 'e', 'f']




```python
x[1][1]
```




    'e'




```python
x[2][0]
```




    'g'



# 第二课作业


```python
fam_height[-1] = 1.68
fam_height
```




    ['father', 1.78, 'mother', 1.68, 'son', 1.8, 'daughter', 1.68]




```python
fam_height[:2] = ['lao wang',1.77]
fam_height
```




    ['lao wang', 1.77, 'mother', 1.68, 'son', 1.8, 'daughter', 1.68]




```python
fam_height =fam_height +['sencond_son',0.51]
fam_height
```




    ['lao wang',
     1.77,
     'mother',
     1.68,
     'son',
     1.8,
     'daughter',
     1.68,
     'sencond_son',
     0.51]




```python
del(fam_height[6:8])
fam_height
```




    ['lao wang', 1.77, 'mother', 1.68, 'son', 1.8, 'sencond_son', 0.51]




```python
fam_height.index(1.77)
```




    1




```python
type(10)
```




    int




```python
type('phone')
```




    str




```python
type(fam_height)
```




    list




```python
int(3.99)
```




    3




```python
str(55)
```




    '55'




```python
print('lao wang is ' + str(55) + ' yesrs old')
```

    lao wang is 55 yesrs old



```python
len(fam_height)
```




    8




```python
list(range(0,9))
```




    [0, 1, 2, 3, 4, 5, 6, 7, 8]




```python

```


```python
names = ['小赵','小钱','小孙','小李','小王','小张']
```


```python
friends = [45, 100, 67, 136, 77, 17]
```


```python

```


```python
for word in words:
    index = names.index(word)
    friends[index] = names[index]
    

```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-61-e44467bd5894> in <module>()
    ----> 1 for word in words:
          2     index = names.index(word)
          3     friends[index] = names[index]
          4 


    NameError: name 'words' is not defined


# 第二课 作业2 ——黄志华


```python
names = ['小赵','小钱','小孙','小李','小王','小张']
friends = [45, 100, 67, 136, 77, 17]
```


```python
Maxfriends = None
Maxnames = None

for i in range(len(names)):
    if Maxfriends is None or friends[i] > Maxfriends :
        Maxfriends = friends[i]
        Maxnames = names[i]
        
print(Maxnames,Maxfriends)
```

    小李 136



```python
Minfriends = None
Minnames = None

for i in range(len(names)):
    if Minfriends is None or friends[i] < Minfriends :
        Minfriends = friends[i]
        Minnames = names[i]
        
print(Minnames,Minfriends)
```

    小张 17



```python
print("微信好友最多的是 " + Maxnames + ",好友数为 " + str(Maxfriends))
print("微信好友最少的是 " + Minnames + ",好友数为 " + str(Minfriends))
```

    微信好友最多的是 小李,好友数为 136
    微信好友最少的是 小张,好友数为 17


## how to insert one line after a match

### case

insert one line after the line which matches some regex rules

### input

file: 

- name: input.txt
- content: 

```
mykey=one
anothervalue=two
lastvalue=three
```

### shell commands

```
sed '/^anothervalue=.*/a after=me' test.txt
```

### output

standrad output

```
mykey=one
anothervalue=two
after=me
lastvalue=three
```

## ref

1. (https://fabianlee.org/2018/10/28/linux-using-sed-to-insert-lines-before-or-after-a-match/)[https://fabianlee.org/2018/10/28/linux-using-sed-to-insert-lines-before-or-after-a-match/]

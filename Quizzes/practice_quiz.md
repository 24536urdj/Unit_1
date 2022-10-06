# Practice 
```.py 
def count_letter(msg,letter:str):
  count = 0 
  for i in range(len(msg)) :
    if msg[i] == letter :
      count+= 1 
  return count
out = count_letter("hello","l")
print(out)
```

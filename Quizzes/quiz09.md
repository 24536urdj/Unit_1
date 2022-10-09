#Quiz 09
def convert(b) :
  for i in range(len(b)) :
    a = ord(b[i]) + 13
    if a > 122 :
      print(chr(a - 26),end="")
    else :
      print(chr(a),end="")
convert("hello world")

![](https://github.com/24536urdj/Unit_1/blob/main/Quizzes/Screen%20Shot%202022-10-09%20at%2019.44.56.png)

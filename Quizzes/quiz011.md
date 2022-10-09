## quiz 011 
    def calendar(a):
      n = 1
      print(" sun,Mon,Tue,wed,Thur,Fri,Sat")
      for week in range(4):
        for day in range(7) :
          print(f"{n:4d}",end="")
          n+= 1
        print(" ")
      print(" " ,29,"",30,"",31)
    calendar(10)
![](https://github.com/24536urdj/Unit_1/blob/main/Quizzes/Screen%20Shot%202022-10-10%20at%203.15.39.png)

## quiz015
     def door(N) :
        count = 1
        for i in range(1,N+1) :
          output = False  
          if N%i == 0 :
            output = True  
            count += 1
            print(count)

    door(5)
![](https://github.com/24536urdj/Unit_1/blob/main/Quizzes/Screen%20Shot%202022-10-10%20at%203.17.01.png)

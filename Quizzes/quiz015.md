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


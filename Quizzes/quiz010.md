# Quiz
## def power(a):
    for i in range(-12,13,3) :
      n = a*(10**i)
      if n == 1e-12 :
        print(n,"pico")
      else :
        if n == 1e-09 :
          print(n,"nano")
        else :
          if n == 1e-06 :
            print(n,"micro")
          else :
            if n == 0.001 :
              print(n,"mill")
            else :
              if n == 1 :
                print(n,"unit")
              else :
                if n == 1000 :
                  print(n,"kilo")
                else :
                  if n == 1000000 :
                    print(n,"mega")
                  else :
                    if n == 1000000000 :
                      print(n,"giga")
                    else :
                      if n == 10**12 :
                        print(n,"tera")
        

## power(1)

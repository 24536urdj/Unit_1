## Task02
     print("Welcome to EV calculator ")
    a = int(input(''' please choose one of these options 
    1.1. Average time per kWh
    2. Total kWh
    3. Total charge time
    4. Show all data '''))
    if a == 1:
        points = []
        with open("charging_log.csv") as file:
            data = file.readlines()
            values = '''8.878 Kwh
    3.533 Kwh
    6.828 Kwh '''
            print(values)
    with open("charging_log.csv") as file:
        ev_logs = file.readlines()
    if a == 2:
        index = 1
        total_energy = 0
        for log in ev_logs:
            if index > 0:
                values = log.split(",")
                date = values[0]
                energy = values[1]
                time = values[2]
                total_energy += float(energy[0:5])
                index += 1
        print(f"The total energy charged is {total_energy}kWh")
    if a == 3:
        index = 2
        total_charge_time = 0
        for log in ev_logs :
            if index > 0 :
                values = log.split(",")
                date = values[0]
                energy = values[1]
                time = values[2]
                total_charge_time += float(time[0:5])
                index += 1
        print(f"total charge time is {total_charge_time}")


    if a == 4:
        points = []
        with open("charging_log.csv") as file:
            data = file.readlines()
            for line in data:
                print(line)
![](https://github.com/24536urdj/Unit_1/blob/main/Quizzes/Screen%20Shot%202022-10-10%20at%203.45.36.png)
![](https://github.com/24536urdj/Unit_1/blob/main/Quizzes/Screen%20Shot%202022-10-10%20at%203.47.06.png)

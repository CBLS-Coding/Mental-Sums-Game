import random
diff = ""
diff1 = ""
diff2 = ""



while True:
    #Addition
    sign = input("Would You Like Subtraction, Addition or Multiplication?:(Some Answers Can Be Negative!)").lower()
    if sign == "addition":
        while diff != "easy" or diff != "hard" or diff != "quit":
            diff = input("Easy or Hard? Type Quit to Exit").lower()
            if diff == "easy":
                for i in range(5):
                    Num1Aeasy = random.randint(50,100)
                    Num2Aeasy = random.randint(50,100)
                    AnsAeasy = input("What is " + str(Num1Aeasy) + "+" + str(Num2Aeasy) + "?:")
                    while not AnsAeasy.isdigit():
                        print("Invalid, numbers only!")
                        AnsAeasy = input("What is " + str(Num1Aeasy) + "+" + str(Num2Aeasy) + "?:")
                    if AnsAeasy == Num1Aeasy + Num2Aeasy:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Aeasy+Num2Aeasy))
            elif diff == "hard":
                for i in range(5):
                    Num1Ahard = random.randint(150,300)
                    Num2Ahard = random.randint(150,300)
                    AnsAhard = input("What is " + str(Num1Ahard) + "+" + str(Num2Ahard) + "?:")
                    while not AnsAhard.isdigit():
                        print("Invalid, numbers only!")
                        AnsAhard = input("What is " + str(Num1Ahard) + "+" + str(Num2Ahard) + "?:")
                    if AnsAhard == Num1Ahard + Num2Ahard:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Ahard+Num2Ahard))
            elif diff == "quit":
                break
            else:
                print("Invalid, try again")
                continue

    #Subtraction    
    elif sign == "subtraction":
        while diff1 != "easy" or diff1 != "hard" or diff1 != "quit":
            diff1 = input("Easy or Hard? Type Quit to Exit").lower()
            if diff1 == "easy":
                for i in range(5):
                    Num1Seasy = random.randint(50,100)
                    Num2Seasy = random.randint(50,Num1Seasy)
                    AnsSeasy = input("What is " + str(Num1Seasy) + "-" + str(Num2Seasy) + "?:")
                    while not AnsSeasy.isdigit():
                        print("Invalid, numbers only!")
                        AnsSeasy = input("What is " + str(Num1Seasy) + "-" + str(Num2Seasy) + "?:")
                    if int(AnsSeasy) == Num1Seasy - Num2Seasy:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Seasy-Num2Seasy))
            elif diff1 == "hard":
                for i in range(5):
                    Num1Shard = random.randint(150,300)
                    Num2Shard = random.randint(150,Num1Shard)
                    AnsShard = input("What is " + str(Num1Shard) + "-" + str(Num2Shard) + "?:")
                    while not AnsShard.isdigit():
                        print("Invalid, numbers only!")
                        AnsShard = input("What is " + str(Num1Shard) + "-" + str(Num2Shard) + "?:")
                    if int(AnsShard) == Num1Shard - Num2Shard:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Shard-Num2Shard))
            elif diff1 == "quit":
                break
            else:
                print("Invalid, try again")
                continue

    #Multiplication #need try except/check for strings for the questions
    elif sign == "multiplication":
        while diff2 != "easy" or diff2 != "hard" or diff2 != "quit":
            diff2 = input("Easy or Hard? Type Quit to Exit").lower()
            if diff2 == "easy":
                for i in range(5):
                    Num1Measy = random.randint(2,10)
                    Num2Measy = random.randint(2,10)
                    AnsMeasy = input("What is " + str(Num1Measy) + "x" + str(Num2Measy) + "?:")
                    while not AnsMeasy.isdigit():
                        print("Invalid, numbers only!")
                        AnsMeasy = input("What is " + str(Num1Measy) + "x" + str(Num2Measy) + "?:")
                    if int(AnsMeasy) == Num1Measy * Num2Measy:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Measy*Num2Measy))
            elif diff2 == "hard":
                for i in range(5):
                    Num1Mhard = random.randint(2,9)
                    Num2Mhard = random.randint(11,20)
                    AnsMhard = input("What is " + str(Num1Mhard) + "x" + str(Num2Mhard) + "?:")
                    while not AnsMhard.isdigit():
                        print("Invalid, numbers only!")
                        AnsMhard = input("What is " + str(Num1Mhard) + "x" + str(Num2Mhard) + "?:")
                    if int(AnsMhard)== Num1Mhard * Num2Mhard:
                        print("Correct!")
                    else:
                        print("Incorrect! The correct answer was " + str(Num1Mhard*Num2Mhard))
            elif diff2 == "quit":
                break
            else:
                print("Invalid, try again")
                continue
    
    elif sign == "quit":
        print("exiting game")
        break

    else:
        print("Invalid, try again")
        continue





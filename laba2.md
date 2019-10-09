name = None
a = 0
while True:
    print ("Menu")
    print("1. Enter name:")
    print("2. Print greting ")
    print("3. Count the number of letters in words:  ")
    print("4. Quit")

    response = input("Please chose an action:  ")
    
    print("")
    if response == "1":
     name = input("Enter your name: ")
    elif response == "2":
        if name :
            print ("Hello, ",name , "!")
        else :
            print("I dont know your name.")
    elif response == "3":
        s = input("Enter string: ")
        letters = [0]* 26
        for i in s.lower():
          if 'a'<=i<='z':
             number = ord(i)-97
             letters[number]+=1
        for i in range(26):
          if letters[i]>0:
            print(chr(i+97), letters[i])


    elif response == "4":
        break
    else:
         input("Incorect chose! ")

         
    print("")

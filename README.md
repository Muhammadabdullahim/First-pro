# First-pro
user_name = "A"
pin_code = "123"
balance = 100000

user = input("Enter your user name: ")
pin = input("Enter your Pin Code: ")

if user == user_name and pin == pin_code:
    print("1. Balance Inquiry")
    print("2. Cash Deposit")
    print("3. Cash Withdrawl")
    print("4. Exit")
    option = input("Choose Your Option: ")
    if option == "1":
        print(balance)
    elif option == "2":
        deposit_amount = int(input("Enter deposit amount: "))
        print("you balance is ", deposit_amount+balance)
    
    elif option == "3":
        Withdrawl_amount = int(input("Enter withdrawl amount: "))
        if Withdrawl_amount > balance:
            print("Insufficient Balance")

        else:
            print("you balance is ", balance-Withdrawl_amount)
          
    elif option == "4":
        print("Thanks For Using Our Services")  
    else:
        print("Choose Correct Option") 
else:
    print("Invalid")
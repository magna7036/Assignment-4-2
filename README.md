# prompt the user to enter the employee's name, number of shifts worked, 
#number of transactions, and transaction dollar value
name = input("Enter employee's name: ")
shifts = int(input("Enter number of shifts worked: "))
transactions = int(input("Enter number of transactions: "))
dollars = float(input("Enter transaction dollar value: "))

# calculate the productivity score
score = dollars/transactions/shifts

# calculate the bonus based on the productivity score using a nested if statement
if score >= 200:
    bonus = 200.00
elif score >= 70:
    bonus = 100.00
elif score >= 31:
    bonus = 75.00
else:
    bonus = 50.00

# output the employee's name and bonus
print("\nEmployee Name:", name)
print("Employee Bonus: $" + str(bonus))

# 100days-of-coding-in-Python
#TIP GENERATOR
#If the bill was $150.00, split between 5 people, with 12% tip. 
#Each person should pay (150.00 / 5) * 1.12 = 33.6
#Format the result to 2 decimal places = 33.60
#Tip: You might need to do some research in Google to figure out how to do this.

print("Welcome to the Tip Calculator.")
bill_amt = input("What was the total bill?")
tip = input("What percentage tip would you like to give? 10, 12 or 15?")
num = input("How many people to split the bill?")

t = float(tip)/100
total_tip_amount = float(bill_amt) * t
total_bill = float(bill_amt) + float(total_tip_amount)
bill_per_person = float(total_bill) / float(num)
result = round(bill_per_person, 2)


print(f"Each person should pay: {result}") 

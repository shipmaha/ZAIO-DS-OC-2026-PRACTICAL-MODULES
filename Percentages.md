Task 1: Percentages
Provide evidence, then save before moving on.

Question 1: Discount Calculator

Write a Python program that asks the user to enter the original price of an item and the discount percentage. The program must calculate the discount amount and the final price after applying the discount, then display both results. (5 marks)

original_price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

discount_amount = original_price * discount_percent / 100
final_price = original_price - discount_amount

print(f"Discount amount: {discount_amount:.2f}")
print(f"Final price: {final_price:.2f}")

Question 2: Exam Percentage and Grade

Write a Python program that asks the user to enter the marks obtained and the total marks. The program must calculate the percentage and display it. Based on the percentage, print the grade as follows: 75% and above is Distinction, 60%–74% is Merit, 50%–59% is Pass, and below 50% is Fail. (5 marks)

marks_obtained = float(input("Enter the marks obtained: "))
total_marks = float(input("Enter the total marks: "))

percentage = (marks_obtained / total_marks) * 100
print(f"Percentage: {percentage:.2f}%")

if percentage >= 75:
    print("Grade: Distinction")
elif percentage >= 60:
    print("Grade: Merit")
elif percentage >= 50:
    print("Grade: Pass")
else:
    print("Grade: Fail")

Question 3: Salary Increase

Write a Python program that asks the user to enter their current salary and the percentage increase. The program must calculate the increase amount and the new salary after the increase, then display both values. (5 marks)

current_salary = float(input("Enter your current salary: "))
increase_percentage = float(input("Enter the percentage increase: "))

increase_amount = current_salary * (increase_percentage / 100)
new_salary = current_salary + increase_amount

print(f"Increase amount: {increase_amount:.2f}")
print(f"New salary: {new_salary:.2f}")

Question 4: Profit Percentage

Write a Python program that asks the user to enter the cost price and the selling price of an item. The program must calculate the profit or loss and then calculate the percentage using the formula: Profit % = (Profit ÷ Cost Price) × 100. The program should display whether it is a profit or a loss and show the percentage. (5 marks)

cost_price = float(input("Enter the cost price: "))
selling_price = float(input("Enter the selling price: "))

profit = selling_price - cost_price
percentage = (profit / cost_price) * 100

if profit > 0:
    print(f"Profit: {profit:.2f}")
    print(f"Profit percentage: {percentage:.2f}%")
elif profit < 0:
    print(f"Loss: {abs(profit):.2f}")
    print(f"Loss percentage: {abs(percentage):.2f}%")
else:
    print("No profit or loss.")
Task 1: Dividing two integers
Provide evidence, then save before moving on.

1.1 - Provide python 3 code for a function distribute_n() that takes in an integer number n, and an integer number k as arguments,then returns a list with k-elements such that the sum of the elements in the list is equal to n. If n is not greater than or equal to k, the function must return None. The elements of the list are required to be at least 1. (5 marks)

def distribute_n(n, k):
    if k <= 0 or n < k:
        return None
    
    base_value = n // k
    remainder = n % k
   
    result = [base_value] * k
    
    for i in range(remainder):
        result[i] += 1
        
    return result

1.2 - Provide python 3 code for a function pie_chart() that takes in a list (“percentages[]”) of real numbers between 0 and 100, and uses the numbers in the list as percentages 

and return a list of tuples (p, share) where p is the number in the list, and share is a percentage of out 360. If the numbers in percentages[] do not add up to 100 exactly, 

return None. (5 marks)

def pie_chart(percentages):
  if sum(percentages) != 100:
    return None
 
  result = [(p, (p / 100) * 360) for p in percentages]
  return result


1.3 - Provide python 3 code for a function school_trip() that takes a number n, which represents the number of students going on a trip, and returns a list of tuples (“taxi n:”, k) where “taxi n:” is the taxi number, and k is the number of students in that taxi. (5 marks)

def school_trip(n, capacity=15):
    if n < 0:
        return None

    taxis = []
    taxi_number = 1

     while n > 0:        
        students_in_taxi = min(n, capacity)
        taxis.append((f"taxi {taxi_number}:", students_in_taxi))
        
        n -= students_in_taxi
        taxi_number += 1

    return taxis    
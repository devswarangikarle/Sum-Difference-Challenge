# Sum-Difference-Challenge

In a small town, a math enthusiast named Aryan discovered a peculiar array filled with numbers. Curious about the relationship between even and odd numbers, he decided to explore further. With N integers in hand, Aryan set out to calculate the sum of all even numbers and the sum of all odd numbers in the array. His goal was to find the absolute difference between these two sums. Can you help Aryan uncover the mystery hidden in the numbers?

Input
The first line of the input contains a single integer N.
The second line of the input contains N space-separated integers.

Constraints
1 ≤ N ≤ 10^5
1 ≤ Ai ≤ 10^9
Output
Print the absolute difference in sums of even numbers and odd numbers in the array.

# Input reading
N = int(input())  # Number of integers
numbers = list(map(int, input().split()))  # Array of N integers

# Initializing sums
sum_even = 0
sum_odd = 0

# Iterating through the numbers
for num in numbers:
    if num % 2 == 0:  # Check if the number is even
        sum_even += num
    else:  # Otherwise, it's odd
        sum_odd += num

# Calculate the absolute difference
result = abs(sum_even - sum_odd)

# Print the result
print(result)

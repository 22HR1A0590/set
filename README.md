# set

'''1) Write a program to get n number of values in separate line for set and print the values with space separation.
Sample Input:
5
3
1
4
5
2
Sample Output:
1 2 3 4 5 
Note: There is trailing space at the end of output'''

Ans:
n = int(input())
values_set = set()
for _ in range(n):
    value = int(input())
    values_set.add(value)
sorted_values = sorted(values_set)
print(" ".join(map(str, sorted_values)) + " ")

'''2) Write a program to get input in a single line separated by space and print the values of set in single line separated by space.
Sample Input:
3 1 5 4 2
Sample Output:
1 2 3 4 5
Note: There is no trailing space at the end of output.'''

Ans:
input_values = input()
values_set = set(map(int, input_values.split()))
sorted_values = sorted(values_set)
print(" ".join(map(str, sorted_values)))

'''3) Write a program to print only the different values between two given sets.
Sample Input:
1 2 3 4
2 4 6 8
Sample Output:
1 3
Note: There are trailing spaces at the end of output.'''

Ans:
set1_input = input()
set1 = set(map(int, set1_input.split()))
set2_input = input()
set2 = set(map(int, set2_input.split()))
difference = set1.difference(set2)
sorted_difference = sorted(difference)
print(" ".join(map(str, sorted_difference)) + " ")

'''4) Write a program to delete the given element in the given set values. If the given element is not in the set values, then print "Given value is not present in the set list.".
Sample Input:
1 2 3 4
2
Sample Output:
1 3 4 
Note: There is a trailing space at the end of the list.'''

Ans:
set_input = input()
values_set = set(map(int, set_input.split()))
element_to_delete = int(input())
if element_to_delete in values_set:
    values_set.remove(element_to_delete)
    sorted_values = sorted(values_set)
    print(" ".join(map(str, sorted_values)) + " ")
else:
    print("Given value is not present in the set list.")

'''5) Write a program to print the values which are similar in both given sets.
Sample Input:
1 2 3 4
2 4 6 8
Sample Output:
2 4 
Note: Trailing spaces are there at the end of the output.'''

Ans:
set1_input = input()
set1 = set(map(int, set1_input.split()))
set2_input = input()
set2 = set(map(int, set2_input.split()))
common_values = set1.intersection(set2)
sorted_common_values = sorted(common_values)
print(" ".join(map(str, sorted_common_values)) + " ")

'''6)
Write a program to get the set values in a single line separated by space (including duplicate values) and print the number of elements in the given set.
Sample Input:
1 2 3 4 5 1 2 3
Sample Output:
5'''

Ans:
input_values = input()
values_set = set(map(int, input_values.split()))
num_elements = len(values_set)
print(num_elements)

'''7) Write a program to find the maximum and minimum value of given set values.
Sample Input:
1 2 3 4 5
Sample Output:
Maximum: 5
Minimum: 1'''

Ans:
input_values = input()
values_set = set(map(int, input_values.split()))
max_value = max(values_set)
min_value = min(values_set)
print(f"Maximum: {max_value}")
print(f"Minimum: {min_value}")

'''8) Write a program to update the given set in another set.
Sample Input:
1 2 3
3 4 5
Sample Output:
1 2 3 4 5'''

Ans:
set1_input = input()
set1 = set(map(int, set1_input.split()))
set2_input = input()
set2 = set(map(int, set2_input.split()))
set1.update(set2)
sorted_updated_set = sorted(set1)
print(" ".join(map(str, sorted_updated_set)))

'''9) Write a program to get set values in a single line with space(including duplicate values) and find the number of duplicate values given during input and print the output set value without duplicate elements.
Sample Input:
6
1
2
1
2
3
1
Sample Output:
Duplicate Values: 3
1 2 3 '''

Ans:
















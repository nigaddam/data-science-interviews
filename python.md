# Python examples

# Write a function to returns a list of all the duplicate elements from the input list
# Example 
input_list = [67, 3, 48, 94, 19, 7, 94, 55, 19, 3]
output_list =  [3, 94, 19]

  ``` 
output_list = []

def return_func(list):
    for i in range(0,len(input_list)):
        # print(i)
        for j in range(i+1, len(input_list)):
            if input_list[i] == input_list[j]:
                output_list.append(input_list[i])
            else:
                continue

    return(print(output_list))

return_func(input_list)
  ``` 
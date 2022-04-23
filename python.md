# Python examples

# Write a function to returns a list of all the duplicate elements from the input list
<!-- Example  -->
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

# Add the prime factorials of a number
<!-- f(25) = 5 -->
<!-- f(10) = 7 -->
<!-- f(15) = 8 -->
``` 
def find_prime_factores(n):
    list_prime = []
    i = 2
    while n>1:
        if n%i ==0:
            list_prime.append(i)
            n=n/i
            i=i-1
        i=i+1
    return(list_prime)

list_prime = find_prime_factores(25)

unique_list = []

for num in list_prime:
    if num not in unique_list:
        unique_list.append(num)

print('full list', list_prime)

print('unique list:', unique_list)

print('result: ', sum(unique_list))
``` 



# checking for the winner of the tic tac toe game
``` 
def check_if_winner(self, tic_tac_toe):

    human = 0
    computer = 0

    # row
    for row in range(self.row):
        count = 0
        for col in range(self.column):
            if tic_tac_toe[row][col] == "x" and tic_tac_toe[row][col] != " ":
                count += 1
            else:
                pass
        if count == self.column:
            human += 1
            return True

    # column

    for col in range(self.column):
        count = 0
        for row in range(self.row):
            if tic_tac_toe[row][col] == "x" and tic_tac_toe[row][col] != " ":
                count += 1

            else:
                pass
            if count == self.column:
                human += 1

                return True

    # diagonal

    count = 0
    for col in range(self.column):
        # count = 0
        for row in range(self.row):
            if row == col and tic_tac_toe[row][col] != " ":
                if tic_tac_toe[row][col] == "x":
                    count += 1
            else:
                pass
            if count == self.column:
                human += 1

                return True

    count = 0
    sum = self.column
    for row in range(self.row):
        for col in range(self.column):
            if (col + row) == (sum - 1) and tic_tac_toe[row][col] != " ":
                if tic_tac_toe[row][col] == "x":
                    count += 1
            else:
                pass
    if count == self.column:
        human += 1

        return True

    # checking for the winner
    if computer or human == 1 and self.total_chances < self.chance:
        if human > computer:
            print("human wins")
        elif computer > human:
            print("computer wins")
        else:
            print("match draw")
```             
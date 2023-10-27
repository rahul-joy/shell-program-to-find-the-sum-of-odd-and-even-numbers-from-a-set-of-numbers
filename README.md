# shell-program-to-find-the-sum-of-odd-and-even-numbers-from-a-set-of-numbers



-----------------------------|

#!/bin/bash

even_sum=0
odd_sum=0

echo "Enter numbers (separated by spaces):"
read input

numbers=($input)

for number in "${numbers[@]}"; do
    if ((number % 2 == 0)); then
        even_sum=$((even_sum + number))
    else
        odd_sum=$((odd_sum + number))
    fi
done

echo "Sum of even numbers: $even_sum"
echo "Sum of odd numbers: $odd_sum"

------------------------|

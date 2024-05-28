#!/bin/bash

# Function to check if a string is a palindrome
is_palindrome() {
    local str="$1"
    local length=${#str}
    local half_length=$((length / 2))

    for (( i = 0; i < half_length; i++ )); do
        if [ "${str:i:1}" != "${str:length-i-1:1}" ]; then
            return 1
        fi
    done
    return 0
}

# Read input from the user
read -p "Enter a string: " input_string

# Call the is_palindrome function
if is_palindrome "$input_string"; then
    echo "\"$input_string\" is a palindrome."
else
    echo "\"$input_string\" is not a palindrome."
fi

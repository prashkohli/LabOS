#!/bin/bash

string="This is a sample string to search"
substring="sample"

# Use grep to search for the substring in the string
if grep -q "$substring" <<< "$string"; then
    echo "Substring '$substring' found in the string."
    positions=$(grep -bo "$substring" <<< "$string" | cut -d ":" -f 1)
    echo "Positions of occurrences: $positions"
else
    echo "Substring '$substring' not found in the string."
fi

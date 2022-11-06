#!/bin/bash

echo "Please Select question"
read qNum
if [[ qNum -eq 1 ]]
then
echo "Write the first number Please"
read  firstNum
echo "Write the second number please"
read   secondNum

sum=$(echo "$firstNum + $secondNum" | bc)

if [[ $sum -gt 100 ]]
then
        echo "The sum of the two numbers greater  than 100"
elif [[ $sum -lt 100 ]]
then
        echo "The sum of the two numbers is less than 100"
else
        echo "The sum of the two numbers is equal to 100"
fi

elif [[ qNum -eq 3 ]]
then
read -p "please enter the path of your directory" path
find $path -type f | du -a | sort -n -r | head -n 10

elif [[ qNum -eq 2 ]]
then
read -p  " write a temprature in Fahrenheit"  Ft
Ft=$(($Ft-32))
Celsius=$(echo "scale=2;$Ft*(5/9)" | bc)
echo $Celsius
fi

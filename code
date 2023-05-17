# This program is using if-elif-else statements to calculate interest on an investment or how much they'll need to pay on a loan.
# The user needs to input what they want to calculate and the information needed to calculate that. 
# The program outputs what their interest is if they chose investment or theirmonthly repayment amount if they chose bond.

import math

print("investment - to calculate the amount of interest you'll earn on your investment")
print("bond - to calculate the amount you'll have to pay on a home loan")
print(" ")
print("Enter either 'investment' or 'bond' from the menu above to proceed:")
menuoption = input("").lower()

if menuoption == "investment":
    print("Please fill in the following questions")
    Pinv = float(input("The amount of money being deposited: "))
    interest_rate =input("The interest rate (as a percentage): ")
    r = float(interest_rate)/100
    t = float(input("Number of years you plan on investing: "))
    interest = input("Simple or compound interest? ")

    if interest == "simple":
        simpleinterest = Pinv*(1 + r*int(t))
        print("Your interest is:" + str(simpleinterest))

    elif interest == "compound":
        compoundinterest = Pinv * math.pow((1+r),t) 
        print("Your interest is:" + str(compoundinterest))
    
    else:
        print("Error: Please enter simple or compound")

elif menuoption == "bond":
    Pbond = float(input("The current value of the house:"))
    ann_int = float(input("The interest rate: "))
    i = ((ann_int/100)/12)
    n = float(input("The number of months you plan to take to repay the bond: "))
    repayment = (i*Pbond)/(1-(1+i)**(-n))
    print("Your monthly repayments will be: " + str(repayment))

else:
    print("Error: Please enter investment or bond")

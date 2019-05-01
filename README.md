# pythonFinance
Some python code for financial calculation.

### Calculate compound interest
```
def sumAfterCompoundInterest(principal, interestPerAnnum, compoundingFrequencyPerYear,years):
  return principal*(1+interestPerAnnum/compoundingFrequencyPerYear)**(years*compoundingFrequencyPerYear)

amount = sumAfterCompoundInterest(100,0.02,2,10)
print(amount)
```

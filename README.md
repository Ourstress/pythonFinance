# pythonFinance
Some python code for practical uses eg. financial calculation.

### Calculate compound interest
```
def sumAfterCompoundInterest(principal, interestPerAnnum, compoundingFrequencyPerYear,years):
  return principal*(1+interestPerAnnum/compoundingFrequencyPerYear)**(years*compoundingFrequencyPerYear)

amount = sumAfterCompoundInterest(100,0.02,2,10)
print(amount)
```

### Calculate Body Mass Index
```
def calculateBmiIndex(weightInKg, heightInM):
  return weightInKg/(heightInM**2)

def bmiResults(weightInKg, heightInM):
  bmiIndex = calculateBmiIndex(weightInKg,heightInM)
  if bmiIndex > 22.999:
    return "BMI of {0} outside healthy range :(".format(bmiIndex)
  else:
    return "BMI of {0} within healthy range! :)".format(bmiIndex)

print(bmiResults(40,1.5))
# source: https://www.healthhub.sg/programmes/93/bmi-calculator
```

### Calculate Pollutant Standards Index (PSI)
```
def calculatePsiIndex(PSI):
  if PSI > 0 and PSI < 50:
    return "PSI:{0} - Low air pollution level".format(PSI)
  elif PSI >= 50 and PSI < 100:
    return "PSI:{0} - Moderate air pollution level".format(PSI)   
  elif PSI >= 101 and PSI < 200:
    return "PSI:{0} - unhealthy air pollution level".format(PSI)     
  elif PSI >= 201 and PSI < 300:
    return "PSI:{0} - Very unhealthy air pollution level".format(PSI)     
  elif PSI >= 300:
    return "PSI:{0} - Haxardous air pollution level".format(PSI)      

print(calculatePsiIndex(500))
# Source: https://en.wikipedia.org/wiki/Pollutant_Standards_Index

```

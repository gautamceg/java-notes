## java-notes
[Mastering-markdown](https://guides.github.com/features/mastering-markdown/)
1. **RoundingMode.HALF_UP**
- All totals should be formatted to 2 decimal places, rounded up i.e. 0.567 should result in 0.57 but 0.564 should result in 0.56 [(see this link)](http://www.clivemaxfield.com/diycalculator/sp-round.shtml#A3)
- `BigDecimal.valueOf(amount).setScale(2, RoundingMode.HALF_UP).doubleValue();`

2. **Round Up with Leap**
- If roundUp
- ```double maxRoundValue = Math.ceil(Double.valueOf(maxValue) / Double.valueOf(maxStep)) * Double.valueOf(maxStep);```

3. **How to run specific JUnit test class or method?**
- To execute all tests in a file CircleTest.java
  ```mvn clean package -Dtest=CircleTest```

- To execute specific testMethod() in a file CircleTest.java
  ```mvn clean package -Dtest=CircleTest#testMethod```

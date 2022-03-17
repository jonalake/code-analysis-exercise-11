# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input | Output |
| ----- | ------ |
|   1   |    1, 15, 15    | 
|   2   |    1, 24, 24    | 
|   3   |    3, 28, 29    | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>Program takes input of actualAge and returns that age in humanYears, catYears, and dogYears. For all cases, humanYears equals actualAge. For actual age of 1, catYears and dogYears equals 15.  For actual age of 2, catYears and dogYears equals 24. For all other actualAge inputs, catYears and dogYears follow respective formulas to calculate.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible

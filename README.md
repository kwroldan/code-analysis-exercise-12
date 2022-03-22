# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

*SUMMARY*
1) The function takes an input string `currentColor` and checks it against the next steps.
2) If the `currentColor` is `green`, the `nextColor` is defined as `yellow`. 
3) If Step 2 is false, it checks if `currentColor` is `yellow`. If it is, `nextColor` is defined as `red`.
4) If Step 2 and 3 are false, the function checks if `currentColor` is `red`, and if so, `nextColor` is defined as `green`.
5) The function then returns `nextColor`.

```js
function (currentColor){
  if (currentColor === "green"){
    nextColor = "yellow"
  } else if (currentColor === "yellow"){
    nextColor = 'red'
  } else if (currentColor === "red"){
    nextColor = 'green'
  }

  return nextColor
}
```

Inputs and outputs should be valid JavaScript values!

| Input  | Output |
| ------ | ------ |
| red    | green  | 
| yellow | red    | 
| green  | yellow | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program mirrors the functionality of a traffic light.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible

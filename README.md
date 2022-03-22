# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (person, petName){
  for (let dog of person.dogs){
    if (dog.name === petName){
      return dog
    }
  }
}
```

Inputs and outputs should be valid JavaScript values!

| Input | Output |
| ----- | ------ |
|   `const james = {name: "James", dogs: [{name: "Lily", breed: "Austrlian Shepherd", gender: "female"}] function (james, "Lily")`| `{name: "Lily", breed: "Austrlian Shepherd", gender: "female"}`       | 
|   `const bill = {name: "Bill", dogs: [{name: "Samson", breed: "German Shepherd", gender: "male"}, {name: "Delilah", breed: "Golden Retriever", gender: "female"}] function (bill, "Delilah")`    |  `{name: "Delilah", breed: "Golden Retriever", gender: "female"}`      | 
|       |        | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td></td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible

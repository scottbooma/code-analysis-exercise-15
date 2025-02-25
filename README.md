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
|   `const james = {name: "James", dogs: [{name: "Lily", breed: "Austrlian Shepherd", gender: "female"}] } function (james, "Lily")`| `{name: "Lily", breed: "Austrlian Shepherd", gender: "female"}`       | 
|   `const bill = {name: "Bill", dogs: [{name: "Samson", breed: "German Shepherd", gender: "male"}, {name: "Delilah", breed: "Golden Retriever", gender: "female"}] } function (bill, "Delilah")`    |  `{name: "Delilah", breed: "Golden Retriever", gender: "female"}`      | 
|   `const scott = {name: Scott, cats: [{name: "Lily", breed: "Sweet Girl", gender: "female"}, {name: "Tippur", breed: "Crazy Boy", gender: "male"}] } function (scott, "Tippur")`   |  error      | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program takes an object with one of its properties being an array labeled "dogs" whose items are objects containing information for each dog. It searches the array to see if the name of a dog matches the `petName` input. If it is a match it will return the entire object for the dog that was a match. This works like a `.find` might to search through an array.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible

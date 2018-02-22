# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- Issue-tracker app should store issues array in an object
- The object should have displayIssues method
- The object should have addIssue method
- The object should have changeIssue method
- The object should have deleteIssue method

## Code Snippet

### Issue-tracker app should store issues array in an object
```
 function addIssue(issue){
  issues.push(issue);
  displayIssues();
 }
```

### The object should have displayIssues method
```
 function displayIssues(){
  console.log('My Issues : ',issues);
 }
```

### The object should have addIssue method
```
 function changeIssue(position,newIssue){
  issues[position]=newIssue;
  displayIssues();
 }
```

### The object should have changeIssue method
```
 function deleteIssue(position){
  issues.splice(position,1);
  displayIssues();
 }
```

### The object should have deleteIssue method
```
 function deleteIssue(position){
  issues.splice(position,1);
  displayIssues();
 }
```
## Reference
* [Object - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)


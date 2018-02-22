# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- Your issue-tracker app should have a way to create issues list
- It should have a way to add issue in the issues list
- It should have a way to display issues list
- It should have a way to change an issue in the issues list
- It should have a way to delete an issue from the issues list

## Code Snippet

### Your issue-tracker app should have a way to create issues list
```
 var issues=['issue-1','issue-2','issue-3'];
```
### It should have a way to add issue in the issues list
```
 issues.push('issue-4');
```

### It should have a way to display issues list
```
 console.log('My Issues : ',issues);
```

### It should have a way to change an issue in the issues list
```
 issues[1]='changed';
```

### It should have a way to delete an issue from the issues list
```
 issues.splice(1,1);
```
## Reference
* [Array - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

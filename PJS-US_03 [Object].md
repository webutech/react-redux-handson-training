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

> Concept of :  "Close for Modification and Open for Extention"

## Code Snippet
- Create folder structure
- Create script.js file in js folder
- Create index.html file and include script.js file in script section on index.html page
### Issue-tracker app should store issues array in an object
```
var issueList={
  issues:['Issue-1','Issue-2','Issue-3']  
};
```
### The object should have displayIssues method
```
var issueList={
  issues:['Issue-1','Issue-2','Issue-3'],
  displayIssues:function(){
      console.log('My Issues : '+this.issues);
  }    
};
```

### The object should have addIssue method
```
var issueList={
    issues:['Issue-1','Issue-2','Issue-3'],
  
    displayIssues:function(){
        console.log('My Issues : '+this.issues);
    },
    
    addIssue:function(issue){
        this.issues.push(issue);
        this.displayIssues();
    }  
    
};
 
```

### The object should have changeIssue method
```
var issueList={
    issues:['Issue-1','Issue-2','Issue-3'],
  
    displayIssues:function(){
        console.log('My Issues : '+this.issues);
    },
    
    addIssue:function(issue){
        this.issues.push(issue);
        this.displayIssues();
    },
    
    changeIssue: function(position, newIssue){
        this.issues[position]=newIssue;
        this.displayIssues();
    }
    
};
 
```

### The object should have deleteIssue method
```
var issueList={
    issues:['Issue-1','Issue-2','Issue-3'],
  
    displayIssues:function(){
        console.log('My Issues : '+this.issues);
    },
    
    addIssue:function(issue){
        this.issues.push(issue);
        this.displayIssues();
    },
    
    changeIssue: function(position, newIssue){
        this.issues[position]=newIssue;
        this.displayIssues();
    },
    
    deleteIssue: function(position){
        this.issues.splice(position,1);
        this.displayIssues();
    }
    
};
```
## Reference
* [Object - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)


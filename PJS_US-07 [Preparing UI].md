## Preparing UI
The UI of our application will be as below. 
![Issue-Tracker UI](https://github.com/code-gram/react-redux-handson-training/blob/master/images/IssueTracker-wireframe.png)

## index.html code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Issue Tracker- App</title>
    <link rel="stylesheet" href="css/style.css" type="text/css">
    
</head>
<body>
   <table border="1">
        <tr>
            <td height="25px">
                <h1 class="appTitle">Issue-Tracker-App using [Vanilla Js + HTML + CSS]</h1>
            </td>
        </tr>
        <tr>
            
            <td height="400px" valign="top">
                <div class="container">
                <div>
                    //TODO: Working Area
                </div>
                
                <div id="sideInstruction">
                   <p>Hover on Issue or [X] button to get the help</p>
                   <p>Click on Issue or [X] button to change status or delete Issue</p>
                    
                </div>
                <br/>    
                </div>
                <hr/>
                <ul>
                
                </ul>
                
            </td>
            
        </tr>
        <tr>
            <td height="20px">&reg; Developed by :  Pankaj Sharma</td>
        </tr>
    </table>
    
    <script type="text/javascript" src="js/script.js"></script>
</body>
</html>
```

## style.css code
```
.appTitle{
    color:#218c74;
    background-color: #33d9b2;
    margin: 10px;
    padding: 10px;
    text-shadow: 2px 1px #f7f1e3;
}

body{
    background-color: #ecf0f1;
}
.container{
    margin: 10px;
    position:relative;
}

.deleteTodoButton{
    float: right;
}
li{
    list-style: none;
    margin: 10px;
    color: #ecf0f1;
    background-color: #2980b9;
    padding: 10px;
    font-size: 18px;
    font-weight: 100;
    width: 40%
}

#sideInstruction{
    position: absolute;
    top: 0px;
    right: 5px;
    width: 40%;
    background-color: #16a085;
}

#sideInstruction p{
    margin:10px;
    color:#ecf0f1;
}


table{
    width:80%;
    margin: 0 auto;
}
```

# jsfilevalidation.github.io

### JS Code:
```JavaScript

document.getElementById("file").addEventListener('change', function(e){
        let x = e.target.value
        //console.log(x.substring(x.lastIndexOf('.') + 1));
        console.log(x.split(".").at(-1))
        if(x.split(".").at(-1)!='pdf'){
            
            document.getElementById("msg").style.display="block";
            document.getElementById("button").disabled = true;
        }
        else{
            document.getElementById("msg").style.display="none";
            document.getElementById("button").disabled = false;
        }
    })
```

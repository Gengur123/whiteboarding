// ex. input "aaabccddddaaa"
// ex. output "3ab2c4da"

// Has to keep track of 2 things, 1 is the letters and how much it appears consecutively


`function compress(str){
  //stores the results and counter
    let result = ''
    let counter = 0;
    
    for (let i = 0; i < str.length; i++){
        counter ++
        //checks if the next letter is different if so it returns the result + counter the goes back in the loop and checks the next letter
        
        if (str[i] != str[i + 1]) {
            if (counter === 1)
                counter = ""
            result = result + counter + str[i];
            
        counter = 0; 
        }
    }
    console.log(result)
    return result
}
`
compress("aaabccddddaaa")


// Ran out of time
```function recursive (string, i = 0, result = ''){
    if (i >= string.length){
        return result
    } else if (string[i] != str[i + 1]){
        
    } else {
        return recursive (string, i+1 result)
    }
        
}
```

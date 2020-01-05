# KatasDelivery

## Numbers to Letters

```javascript

function switcher2(x){

       let finalstring = "";
      //Creo un array con todas las letrras
      let letterarray = [" ","?","!","a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z"];
      let chararray = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29];
        //Aqui  genero otro array con los valores del 0 al 29
      chararray.reverse();
 
      
                for(let o = 0; o <=  x.length ;o++){
                  for(let ar = 0; ar <= 28; ar++){

                if(x[o] == chararray[ar] ){

                    finalstring = finalstring + letterarray[ar];

               
                }
                  }
                  }
return  finalstring;
                }

```

  ## Remove first and last
  ```javascript
function removeChar(str){

var final = str.substring(1,str.length -1);

return final;
};

```
 ## Vowel count
  ```javascript
function getCount(str) {
  var vowelsCount = 0;
  
  for( let vow = 0; vow <= str.length;vow++ ){
  
 switch(str[vow]) {
  case "a":
  vowelsCount ++;
  break;
   case "e":
  vowelsCount ++;
    break;
 case "i":
  vowelsCount ++;
    break;
   case "o":
  vowelsCount ++;
    break;
   case "u":
  vowelsCount ++;
    break;
}


  
  }
  // enter your majic here
  
  return vowelsCount;
}

```

 ## Count positives sum negatives
  ```javascript
function countPositivesSumNegatives(input) {

let out = [0,0];


for(let i = 0; i <= input.length;i++){

if(input[i] > 0 ){
 out[0]++;

}else if (input[i] < 0 ) {
  out[1] = out[1] + input[i];
} if (input[i] ==  "" || input[i] == null  ) {
  console.log("Error");
}
}


    return out;
}
countPositivesSumNegatives([]);
```

 ## Get the mean of the array

  ```javascript
function getAverage(marks){

let averagenote = 0;
for(let i = 0; i <= marks.length - 1;i++){
averagenote = averagenote + marks[i];
}
averagenote = averagenote / marks.length;
averagenote = Math.floor(averagenote);
return averagenote ;
}
getAverage([1,2,3,4,5]);
```

 ## Find number divisible
  ```javascript
function divisibleBy(numbers, divisor){
let divinumbers = [];

for(let i = 0; i <= numbers.length- 1;i++){
if(numbers[i] % divisor === 0 ){
  divinumbers.push(numbers[i]);
  
}
}
return divinumbers;
}

divisibleBy([1,2,3,4,5,6], 2);
```

 ## List Filtering
  ```javascript
function filter_list(list) {
 let result = [];

for(let i = 0; i <= list.length- 1;i++){
if(Number.isInteger(list[i]))  {
result.push(list[i]);
}
}
 return result;
}
```

 ## Credit card
  ```javascript
function maskify(cc) {
let result = "" ;



for(let i = 0 ; i <=  cc.length -5 ;i++){
 result += "#";
}
for(let i  =  cc.length -4 ; i <=  cc.length -1 ;i++){
  if(cc[i] == undefined){

  }else{
 result += cc[i];
  }

}
return result;
}

maskify("4556364607935616");
/*
if(cc[cc.length -1] == cc[cc.length -1] ){

  result += cc[i];
}
*/
```

 ## Flatten
  ```javascript
var flatten = function (array){

let finalarray = [] ;

  for(let i = 0;i < array.length ;i++){
if(array[0] > 0){
finalarray.push(array[i]);
 }

  for(let j = 0; j < array[i].length;j++){


   if (array[0][j] > 0) {
   finalarray.push(array[i][j]);
   
 }


  }
   

}
return finalarray;

}

```

 ## Train square
  ```javascript
function squareDigits(num){
  //may the code be with you


let string = num.toString();
let resultado =  ""  ;

for(let i = 0; i < string.length;i++ ){


 resultado +=  string[i]  * string[i]  ; 
 
}
 
return resultado;

 
  
}
squareDigits(9119);

```

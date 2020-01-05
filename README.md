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

 ## Remove first and last
  ```javascript

```

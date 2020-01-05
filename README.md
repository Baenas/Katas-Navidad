# Katas-Navidad
Katas Navidad
Count positives sum negatives

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

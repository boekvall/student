# student
function convertToRoman(num){

    /* Makeing sure we are within range */

    if (num <1)   {alert("Out of range");}
    if (num >3999) {alert("Out of range");}



/* Simply find the translation in the grid */

var Thousands = ["","M","MM","MMM"];

var Hundreds  = ["","C","CC","CCC","CD","D","DC","DCC","DCCC","XM"];

var Tens      = ["","X","XX","XXX","XL","L","LX","LXX","LXXX","XC"];

var Units     = ["","I","II","III","IV","V","VI","VII","VIII","IX"];

/* xtract single digit for each row  */
return 
Thousands [num /1000] +
Hundreds[(num % 1000)/100] +
Tens[(num%100)/10] +
Units [num%1];
}



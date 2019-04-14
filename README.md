const iterations = 100; //script will print iterations + 1 numbers (+1 is zero)

function LogNumber(i){
    console.log(i);
}

function LogFizz(i){
    console.log("Fizz");
}

function LogBuzz(i){
    console.log("Buzz");
}

function LogFizzBuzz(i){
    console.log("FizzBuzz");
}

var fizzbuzzpattern = [
    LogFizzBuzz, //15
    LogNumber,  //1
    LogNumber,  //2
    LogFizz,    //3
    LogNumber,  //4
    LogBuzz,    //5
    LogFizz,    //6
    LogNumber,  //7
    LogNumber,  //8
    LogFizz,    //9
    LogBuzz,    //10
    LogNumber,  //11
    LogFizz,    //12
    LogNumber,  //13
    LogNumber  //14
]

console.log(0);
var i=1;
var j=1;
while(i<=iterations){
    j=i%15;
    fizzbuzzpattern[j](i);
    i++;
}


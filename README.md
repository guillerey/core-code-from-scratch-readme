# core-code-from-scratch-readme

# Week 1:

## Week challenges (Tuesday):

### 1. Interpreted And Compiled Programming Languages:
 
#### Compiled Languages:

This languages are converted directly into machine code that the processor can execute result in more
faster and more efficient code. Need to be compilated every time when a change is needed.

#### Interpreted Languages:

This languages needs to be intepreted by a program to read and execute the code, is more slower than
compiled languages but is cross-platform, easier to debug, and test.

### 2. Is Java compiled or interpreted, or both?

A java program is first compiled into bytecode which JRE can understand. ByteCode is then interpreted
by the JVM making it as interpreted language, so yes, Java is both, compiled and interpreted language.


### 3. Pseudocode currency converter

    START
    Currency <-- GET
    Num <-- GET
    ExchangeRate <-- 1 US$ = 0,0000220734 XBT
    Currency * ExchangeRate
    Result <-- ConversionRate
    PRINT Result
    END


## Week challenges (Wednesday)

### 1. Matrix Binary DOB
										
										
1024    512    256      128      64     32      16      8       4       2       1

  1      1      1        1        0      1       1      1       1       1       0    =      1982
										
![image](https://user-images.githubusercontent.com/30531913/162103387-61ee275d-08e0-4098-8ae0-544da5f63535.png)




### 2. MISP


    .data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: "
	      result_message: .asciiz "\nEl resultado es: "

    .text
	      main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2
              syscall

              li $v0, 5
              syscall

              move $t1, $v0

              li $v0, 1
              move $a0, $t0
              syscall

              main:
              li $t1, 
              li $v0, 

              add $t2, $t0, $t1

              li $v0, 4
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t2
              syscall


## Week challenges (Thursday) 

1. Print special numbers exercise

	
		for (let i = 0; i <= 101; i += 2)
			console.log(i);


2. Bad Code exercise
3. Bad Code 2 exercise
4. Follow Git Course


\
\



# Week 2:

## Week challenges (Monday)

1. Follow the github course        **Done**
2. Create an account in Codewars   **Done**
3. Read about: if...else           **Done**   
4. Read about: for                 **Done**  
5. Read about: while               **Done** 
6. Read about: functions           **Done** 

## Week challenges (Tuesday)

1. Multiply exercise
2. ASCII Total exercise
3. Char From ASCII Value exercise
4. Binary Addition exercise
5. Student's Final Grade exercise

## Week challenges (Wednesday) 

1. Holiday VIII - Duty Free exercise
2. Twice As Old exercise
3. Valid Spacing exercise

		function validSpacing(s) {
		  for(let i=0;i<=s.length;i++){
		    if (s[0]==' ' || s[s.length-1]==' '){
		      var validation = false;}
		    else if (s[i]==' ' && s[i+1]==' ' && i>=0 && i<s.length-1 || s[i]==' ' && s[i-1]==' ' && i>0 && i<=s.length-1){
		      var validation = false;}
		  }
		if (typeof(validation) == "undefined"){
		  return true;}
		  else {return false};
		}


4. Fake Binary exercise

## Week challenges (Thursday)

1. Remove All Exclamation Marks From The End Of Sentence exercise

		function remove(inputString) {
			let result = inputString;
				while (result[result.length - 1] === "!"){
  				result = result.slice(0,-1);
			}
  				return result;
			}


2. Vowel Remover exercise
3. Rock Paper Scissors! exercise
4. Persistent Bugger exercise


\




# Week 3:

## Week challenges (Monday)

1. Who Likes It? exercise
2. Bit Counting exercise

		var countBits = function(n) {
   			// make an array with the bit result
   			const base = (n).toString(2).split('');
   
 			  // make a sum with the array and make the index a Number
   				const result = base.reduce((sum, num) => sum + Number(num), 0);
   
  				 return result;
				};



3. Your Order, Please exercise

		function order(words){
		  let arr = words.split(' ')
		  let r = []

		  arr.forEach(word=>{
		    let x = word.split('')
		    let num = x.find(el=>parseInt(el))
		    r.push([word,parseInt(num)]) 
		  })

		  r.sort((a,b)=>a[1]-b[1]).map(x=> x.splice(1,1))
		  return r.join(' ')
		}




## Week challenges (Tuesday)

1. Simple Pig Latin exercise

		function pigIt(str){
		  let newArr = [];
		  let strArr = str.split(" ")
		  strArr.forEach(x => {
		    let wordArr = x.split("")
		    wordArr.push(wordArr[0], 'ay'), wordArr.shift()
		    if (x === "!" || x === "?" || x === "." || x === "," || x === ";"){
		      newArr.push(x)
		    } else {
		      newArr.push(wordArr.join(""))
		    }
		  })
		  return newArr.join(" ")
		}


2. Counting Duplicates exercise

		const duplicateCount = (text) => {
		  const splitString = text.toLowerCase().split("").sort();
		  let results = [];
		  for (let i = 0; i < splitString.length; i++) {
		    if (splitString[i] === splitString[i + 1]) {
		      results.push(splitString[i]);
		    }
		  }
		  const setArray = new Set(results);
		  return setArray.size;
		};
		duplicateCount("aabBcde");
		console.log(duplicateCount("aaabBcde"));


3. Decode The Morse Code exercise

		decodeMorse = function(morseCode){
		  morseCode = morseCode.trim();
		  let refinedData = morseCode.split('   ');
		  let result = [];

		  for (let i = 0; i < refinedData.length; i++) {
		    let temp = refinedData[i].split(' ');
		    for (let j = 0; j < temp.length; j++) {
		      if (MORSE_CODE[temp[j]]) {
			result.push(MORSE_CODE[temp[j]]);
		      }
		    }

		    if (i !== refinedData.length - 1) {
		    result.push(' ');
		    }
		  }
		  return result.join('');
		}


## Week challenges (Wednesday)

1. Valid Parentheses exercise

		function validParentheses(parens) {
		  let openNum = 0;
		  for (let i = 0; i < parens.length; i++){
		    if (parens[i] == "(") {
		      openNum += 1;          
		    } else {
		      openNum -= 1;
		    }
		    if (openNum < 0){
		      return false
		    }   
		  }
		  if (openNum === 0){
		    return true   
		  } else {
		    return false
		  }
		}




2. Convert String To Camel Case exercise

		function toCamelCase(str){
		  let strArray;
		  if (str === ""){
		    return "";
		  }
		  if (str.indexOf("-") !== -1){
		    strArray = str.split("-")
		  } else {
		    strArray = str.split("_")
		  }
		  let ccString = strArray[0];
		  for (let i = 0; i < strArray.length; i++){
		    ccString += capitalize(strArray[i]);
		  }
		  return ccString
		  }
		  let capitalize = (str) => {
		    return str[0].toUpperCase() + str.slice(1);
		}

3. Unique In Order exercise

		var uniqueInOrder=function(iterable){
		  let newArr = []
		  for (i = 0; i < iterable.length; i++){
		    if (iterable[i] != iterable[i+1]){
		      newArr.push(iterable[i])
		    }
		  }
		  return newArr
		}


## Week challenges (Thursday)

1. Fold An Array exercise

2. Encrypt This! exercise

		var encryptThis = function(text) {
		  let arr = text.split(' ');
		  let encrypt = arr.map((str) => {
		    if(str.length == 1) return `${str.charCodeAt()}`;
		    if(str.length == 2) return `${str[0].charCodeAt()}${str[1]}`;
		    let rest = str.slice(1);
		    let restFirst = rest[0];
		    let restLast = rest[rest.length-1];
		    let restRest = rest.slice(1,rest.length-1);
		    return `${str[0].charCodeAt()}${restLast}${restRest}${restFirst}`;
		  });
		  return encrypt.join(' ');
		}

3. Complete your 1st Core Challenge




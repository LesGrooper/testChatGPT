# testChatGPT
nyoba soal logic dari chatGPT

pakai bahasa JavaScript

```
// Online Javascript Editor for free
// Write, Edit and Run your Javascript code using JS Online Compiler

const toUpperString = (str) => {
    console.log("Masukan Huruf")
    console.log(str.toUpperCase())
}
toUpperString("asdf")


//
const findUniqChar = (str) => {
    let temp = '';
    for(var i = 0; i < str.length; i++ ){
        if(temp.includes(str[i]) === false){
            temp += str[i]
        }
    }
    return temp
}
console.log(findUniqChar("Aku Ganteng Banget Asik"))


//
const findNumber = (arr) => {
    let min = arr[0];
    let max = arr[0];
    for(var i = 0; i < arr.length; i++){
        if(arr[i] < min){
            min = arr[i]
        } else if (arr[i] > max) {
            max = arr[i]
        }
    }
    return [min,max]
}
console.log(findNumber([1,2,3,4,5]))


//
const findSum = (arr) => {
    let sum = arr.reduce((acc, curr) => acc += curr);
    console.log(sum)
}
findSum([2,4,55])


const findPrime = (num) => {
    if(!1){
        if(num === 1) return 0;
    for(var i = 0; i <= number/2; i++){
        return 0;
    }
    console.log("Bilangan prima")
    } else{
        console.log("Bukan bilangan prima")
    }
}

findPrime(22)

//
const findNum = (num1, num2) => {
    if(!num1 && !num2){
        return "angka invalid!";
    } else if(num1 > num2){
        return true;
    } else if(num1 < num2) {
        return false;
    } else if(num1 === num2) {
        return false
    }
    console.log(num1, num2)
}

findNum(1,4)
findNum(9,10)
findNum(10,11)

//
const isFirstLastCharEqual = (str) => {
    for(var i = 0; i < str.length/2; i++){
        if(str[i] !== str[str.length-1-i]){
            return false;
        }
    }
    return true
}

console.log(isFirstLastCharEqual("hello")) // false
isFirstLastCharEqual("abcba") // true
isFirstLastCharEqual("xyzxy") // true


//

const isSequential = (arr) => {
    let temp = [];
    for(var i = 0; i < arr.length; i++){
        if(!arr){
            return "invalid number!";
        }else if(arr[0] >= arr[arr.length+1+i]){
            return true;
        }
    }
    return false
}
console.log(isSequential([1, 2, 3, 4, 5])) // true
isSequential([10, 20, 30, 40]) // true
isSequential([5, 10, 15, 13]) // false

//
const findMax = (arr) => {
    let max = arr[0];
    for(let i = 0; i < arr.length; i++){
        if(arr[i] > max){
            max = arr[i]
        }
        return max
    }
}
console.log(findMax([3, 7, 1, 9, 5])) // 9
findMax([20, 10, 30, 50, 40]) // 50


//
const filterOddChar = (str) => {
    if(!str){
            return false
        }
    let temp = '';
    for(let i = 0; i < str.length; i++){
        if(i % 2 === 0) {
            temp += str[i];
        }
    }
    return temp;
}

console.log(filterOddChar("abcdefg")) // "aceg"
filterOddChar("abcde") // "ace"

//
const isPalindrome = (str) => {
    if(!str) {
        return false;
    }
    for(var i = 0; i < str.length/2; i++) {
        if(str[i] !== str[str.length-1-i]){
            return 'bukan palindrome broo'
        }
    }
    return 'palindrome brooo'
}

console.log(isPalindrome("civic"))

//
const countWords = (word) => {
    if(!word) return false;
    console.log(word.split(" ").length)
}
countWords("Aku Ganteng")

//
const findSecondMax = (arr) => {
    let max = Math.max(...arr);
  let secondMax = -Infinity;
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] < max && arr[i] > secondMax) {
      secondMax = arr[i];
    }
  }
  if (secondMax === -Infinity) return false;
  return secondMax;
}
console.log(findSecondMax([1, 2, 3, 4, 5]))


//
const splitString = (text, seperator) => {
    if(!text || !seperator) return false;
    console.log(text.split(seperator))
}
splitString("Hello World!", "H")

//
const commonElements = (arr1, arr2) => {
    for(let i = 0; i < arr1.length; i++){
        //menemukan array ke 1
        for(let j = 0; i < arr2.length; i++){
            if(arr1[i] === arr2[j]) return true;
        }
        return false
    }
}
console.log(commonElements([1, 2, 3, 4, 5], [4, 5, 6, 7, 8]))

//
const shuffleString = (str) => {
    const shuffle = str.split(' ').sort(() => {return 0.5-Math.random()}).join('')
}
console.log(shuffleString("Hello World!"))



```

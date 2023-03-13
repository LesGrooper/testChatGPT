# testChatGPT
nyoba soal logic dari chatGPT

pakai bahasa JavaScript

```
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


const countLetters = (str) => {
  const result = {};
  for (let i = 0; i < str.length; i++) {
    const char = str[i].toLowerCase();
    if (char.match(/[a-z]/i)) {
      if (result[char]) {
        result[char]++;
      } else {
        result[char] = 1;
      }
    }
  }
  return result;
};

const str = "openai indonesia";
console.log(countLetters(str));

// menghitung rata-rata jumlah dalam array

const sumArray = (arr) => {
    const sum = arr.reduce((num, jumlah) => num + jumlah);
    return sum/arr.length
}

console.log(sumArray([3,5,7,9]))


// mensoritir angka dalam array


const numberOfArray = [3, 5, 1, 7, 4];
console.log(numberOfArray.sort())


// menghitung fibonacci dengan value  = 20

const isFibon = (char) => {

    let n1 = 0;
    let n2 = 1;
    let increment;
    
    for(let i = 0; i <= char; i++){
        console.log(n1);
        increment = n1+n2;
        n1 = n2;
        n2 = increment;
    }
}
console.log(isFibon(5))


// menghitung huruf vokal dan konsonan
const isVonKal = (str) => {
    const vowels = "aiueo";
    let vowelCount = 0;
    let consonantCount = 0;
        for (let i = 0; i < str.length; i++) {
            const char = str[i].toLowerCase();
            if (char.match(/[a-z]/i)) {
                if (vowels.includes(char)) {
                vowelCount++;
            } else {
                consonantCount++;
            }
        }
    }
    return {
    vokal: vowelCount,
    konsonan: consonantCount
    };
};

console.log(isVonKal('openai indonesia'));


// menghitung angka terbesar dan terkecil dalam array
const countMinMax = (arr) => {
    let min = arr[0];
    let max = arr[0];
    
    for(let i = 0; i < arr.length; i++){
        if(arr[i] === 0){
            return 0;
        } else if (arr[i] >= max){
            max = arr[i];
        }else if(arr[i] <= min){
            min=arr[i];
        }
    }
    return {
        min: min,
        max: max
    }
}
console.log(countMinMax([3, 5, 1, 7, 4]))


// menghitung angka prima

const isPrime = (num) => {
        if(num % 2 === 0){
            console.log("bukan bilangan prima")
            return false
        } else {
            console.log("bilangan prima")
            return true
        }
    
}

console.log(isPrime(17))

// menghitung nganjil dan genap
const isOddEven = (num) => {
    num % 2 === 0 ?  console.log("genap " + num) : console.log("ganjil " + num)
}
isOddEven(2)


// membalikan kalimat dengan revString
// atau dapat di lakukan dengan:

// const revString = (str) => {
//     const arr = str.split(''); // membuat array dari setiap karakter pada string
//     arr.reverse(); // membalik array
//     return arr.join(''); // menggabungkan kembali array menjadi string
// }

// console.log(revString("openai indonesia"));

const revString = (str) => {
    let temp ='';
    for(let i = str.length-1; i >= 0; i--){
        temp += str[i]
    }
    return temp
}
console.log(revString("openai indonesia"))


// mengecek apakah di dalam array ada angka ganjil, lalu dikalikan dengan 2
const isOddEvenArray = (arr) => {
    if(!arr) return false;
    for(let i = 0; i < arr.length; i++){
        arr[i] % 2 === 0 ? arr[i] = arr[i]/2 :  arr[i] = arr[i] *2
    }
    console.log(arr)
}

isOddEvenArray([1, 2, 3, 4, 5, 6, 7, 8, 9])

// memeriksa apakah ada duplikasi dalam array atau tidak, lalu mengeluarkan output berupa angka yang terduplikasi.
const compareArr = (arr1,arr2) => {
    const duplikasi = arr1.filter((e) => arr2.includes(e));
    return duplikasi
}
const arr1 = [1, 2, 3, 4, 5, 6];
const arr2 = [4, 5, 6, 7, 8, 9];
console.log(compareArr(arr1,arr2))


// menghitung karakter yang ada di dalam string

const countStr = (str) => {
    if(!str) return false;
    let counter = 0;
    for(let i = 0; i < str.length; i++){
        const char = str[i].toLowerCase()
        if(char.match(/[a-z]/i)){
            counter++
        }
    }
    console.log(counter)
}
countStr("openai indonesia")



// memerika nilai genap pada array, lalu mengembalikan nilai dan dikalikan 2
const isEven = (arr) => {
    for(let i = 0; i < arr.length; i++){
        arr[i] % 2 === 0 ? arr[i] = arr[i] * 2 : arr[i] = arr[i] / 2
    }
    console.log(arr)
}
isEven([1, 2, 3, 4, 5, 6, 7, 8, 9])


// memeriksa apakah ada duplikasi dalam nilai array
const isDuplicate = (arr) => {
    return arr.filter((e,i) => arr.indexOf(e) === i)
}
console.log(isDuplicate([1, 2, 3, 4, 3, 5, 6, 7, 8, 1]))

// memerika nilai increment dalam array
const incArray = (arr) => {
    increment = 2;
    initVal = 1;
    temp = [initVal]
    for(let i = 1; i < arr.length; i++){
        initVal += increment;
        temp.push[initVal]
        increment ++
    }
    return temp
}

console.log(incArray([1, 2, 3, 4, 5]))


// mencari duplikasi dalam 1 array
const isDuplicated = (arr) => {
return arr.filter((e,i) => arr.indexOf(e) === i && arr.indexOf(e) !== arr.lastIndexOf(e))
}
console.log(isDuplicated([1, 2, 3, 4, 4, 4, 5, 5, 6, 6, 7]))


//
const descEven = (arr) => {
    return arr.filter((e,i) => arr.indexOf(e) % 2 === 0).sort((a,b) => a > b ? -1 : 1)

}
console.log(descEven([1, 2, 3, 4, 5, 6, 7, 8, 9]))


```

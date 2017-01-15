# Algorithms
* [reverseString](https://www.freecodecamp.com/challenges/reverse-a-string#?solution=%0Afunction%20reverseString(str)%20%7B%0A%2F%2F%20%20%20var%20result%20%3D%20%22%22%3B%0A%2F%2F%20%20%20for(var%20i%20%3D%20str.length%3B%20i%3E%3D%200%3B%20i--)%7B%0A%2F%2F%20%20%20%20%20result%20%2B%3D%20str.charAt(i)%3B%0A%2F%2F%20%20%20%7D%0A%2F%2F%20%20%20return%20result%3B%0A%20%20var%20splitedString%20%3D%20%5B%5D%3B%0A%20%20var%20reversedString%20%3D%20%5B%5D%3B%0A%20%20splitedString%20%3D%20str.split(%22%22)%3B%0A%20%20reversedString%20%3D%20splitedString.reverse()%3B%0A%20%20return%20reversedString.join(%22%22)%3B%0A%7D%0A%0AreverseString(%22hello%22)%3B%0AreverseString(%22Greetings%20from%20Earth%22)%3B%0A).

* [factorializeNumber](https://www.freecodecamp.com/challenges/Factorialize%20a%20Number?solution=%0Afunction%20factorialize(num)%20%7B%0A%20%20if(num%20%3C%200)%7B%0A%20%20%20%20return%20-1%3B%0A%20%20%7D%20else%20if(num%20%3D%3D%3D%200)%20%7B%0A%20%20%20%20return%201%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20return%20(num%20*%20factorialize(num%20-%201))%3B%0A%20%20%7D%0A%7D%0A%0Afactorialize(5)%3B%0A).

* [checkForPalindromes](https://www.freecodecamp.com/challenges/Check%20for%20Palindromes?solution=%0Afunction%20palindrome(str)%20%7B%0A%20%20%2F%2F%20Good%20luck!%0A%20%20%0A%20%20%20%20return%20str.replace(%2F%5B%5CW_%5D%2Fg%2C%20%27%27).toLowerCase()%20%3D%3D%3D%20str.replace(%2F%5B%5CW_%5D%2Fg%2C%20%27%27).toLowerCase().split(%27%27).reverse().join(%27%27)%3B%0A%20%20%0A%20%20%0A%7D%0A%0A%0A%0Apalindrome(%22_eye%22)%3B%0A).

* [findTheLongestWordInString](https://www.freecodecamp.com/challenges/Find%20the%20Longest%20Word%20in%20a%20String?solution=%0Afunction%20findLongestWord(str)%20%7B%0A%20%20str%20%3D%20str.split(%22%20%22).reduce(function%20(accumulator%2C%20currentValue)%20%7B%0A%20%20%20%20return%20accumulator.length%20%3E%20currentValue.length%20%3F%20accumulator%20%3A%20currentValue%3B%0A%20%20%20%20%7D)%3B%0A%20%20return%20str.length%3B%0A%7D%0A%0AfindLongestWord(%22The%20quick%20brown%20fox%20jumped%20over%20the%20lazy%20dog%22)%3B%0A).

* [titleCaseSentence](https://www.freecodecamp.com/challenges/Title%20Case%20a%20Sentence?solution=%0Afunction%20titleCase(str)%20%7B%0A%20%20return%20str.replace(%2F%5Cw%5CS*%2Fg%2C%20function(txt)%20%7B%0A%20%20%20%20return%20txt.charAt(0).toUpperCase()%20%2B%20txt.substr(1).toLowerCase()%3B%0A%20%20%7D)%3B%0A%7D%0A%0AtitleCase(%22I%27m%20a%20little%20tea%20pot%22)%3B%0A).

* [returnLargestNumbersInArrays](https://www.freecodecamp.com/challenges/Return%20Largest%20Numbers%20in%20Arrays?solution=%0Afunction%20largestOfFour(arr)%20%7B%0A%20%20%2F%2F%20You%20can%20do%20this!%0A%20%20var%20LargestArr%20%3D%20%5B%5D%3B%0A%20%20arr.map(function(val)%7B%0A%20%20%20%20var%20result%20%3D%20val.reduce(function(accumulator%2C%20currentValue)%7B%0A%20%20%20%20%20%20return%20(accumulator%20%3E%20currentValue%20%3F%20accumulator%20%3A%20currentValue)%3B%0A%20%20%20%20%20%20%7D)%3B%0A%20%20%20%20LargestArr.push(result)%3B%0A%20%20%20%20%7D)%3B%0A%20%20return%20LargestArr%3B%0A%20%20%7D%0A%0AlargestOfFour(%5B%5B4%2C%205%2C%201%2C%203%5D%2C%20%5B13%2C%2027%2C%2018%2C%2026%5D%2C%20%5B32%2C%2035%2C%2037%2C%2039%5D%2C%20%5B1000%2C%201001%2C%20857%2C%201%5D%5D)%3B%0A).

* [confirmTheEnding](https://www.freecodecamp.com/challenges/confirm-the-ending#?solution=%0Afunction%20confirmEnding(str%2C%20target)%20%7B%0A%20%20%2F%2F%20%22Never%20give%20up%20and%20good%20luck%20will%20find%20you.%22%0A%20%20%2F%2F%20--%20Falcor%0A%20%20return%20str.substring(str.length%20-%20target.length%2C%20str.length)%20%3D%3D%3D%20target%3B%0A%7D%0A%0AconfirmEnding(%22Bastian%22%2C%20%22n%22)%3B%0A).

* [repeatStringRepeatString](https://www.freecodecamp.com/challenges/repeat-a-string-repeat-a-string#?solution=%0Afunction%20repeatStringNumTimes(str%2C%20num)%20%7B%0A%20%20%2F%2F%20repeat%20after%20me%0A%20%20var%20repeatedStr%20%3D%20''%3B%0A%20%20if%20(num%20%3C%200)%20%7B%0A%20%20%20%20return%20repeatedStr%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20for%20(var%20count%20%3D%200%3B%20count%20%3C%20num%3B%20count%2B%2B)%20%7B%0A%20%20%20%20%20%20repeatedStr%20%2B%3D%20str%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20repeatedStr%3B%0A%7D%0A%0ArepeatStringNumTimes(%22abc%22%2C%203)%3B%0A).

* [truncateString](https://www.freecodecamp.com/challenges/truncate-a-string#?solution=%0Afunction%20truncateString(str%2C%20num)%20%7B%0A%20%20%2F%2F%20Clear%20out%20that%20junk%20in%20your%20trunk%0A%20%20if%20(str.length%20%3C%3D%20num)%20%7B%0A%20%20%20%20return%20str%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20return%20str.slice(0%2C%20num%20%3E%203%20%3F%20num%20-%203%20%3A%20num)%20%2B%20'...'%3B%0A%20%20%7D%0A%7D%0A%0AtruncateString(%22A-tisket%20a-tasket%20A%20green%20and%20yellow%20basket%22%2C%2011)%3B%0A).

* [chunkyMonkey](https://www.freecodecamp.com/challenges/chunky-monkey#?solution=function%20chunkArrayInGroups(arr%2C%20size)%20%7B%0A%20%20%2F%2F%20Break%20it%20up.%0A%20%20var%20result%20%3D%20%5B%5D%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%20arr.length%3B%20i%20%3D%20i%20%2B%20size)%20%7B%0A%20%20%20%20result.push(arr.slice(i%2C%20i%20%2B%20size))%3B%0A%20%20%7D%0A%20%20return%20result%3B%0A%7D%0A%0AchunkArrayInGroups(%5B'a'%2C%20'b'%2C%20'c'%2C%20'd'%5D%2C%202)%3B%0A).

* [slasherFlick](https://www.freecodecamp.com/challenges/slasher-flick#?solution=%0Afunction%20slasher(arr%2C%20howMany)%20%7B%0A%20%20%2F%2F%20it%20doesn't%20always%20pay%20to%20be%20first%0A%20%20arr.splice(0%2C%20howMany)%3B%0A%20%20return%20arr%3B%0A%7D%0A%0Aslasher(%5B1%2C%202%2C%203%5D%2C%202)%3B%0A).

* [mutations](https://www.freecodecamp.com/challenges/mutations#?solution=%0Afunction%20mutation(arr)%20%7B%0A%20%20var%20str0%20%3D%20arr%5B0%5D.toLowerCase().split('')%3B%0A%20%20var%20str1%20%3D%20arr%5B1%5D.toLowerCase().split('')%3B%0A%20%20var%20count%20%3D%200%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%20str1.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(str0.indexOf(str1%5Bi%5D)%20%3E%20-1)%20%7B%0A%20%20%20%20%20%20count%2B%2B%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20count%20%3D%3D%3D%20str1.length%3B%0A%7D%0A%0Amutation(%5B%22hello%22%2C%20%22hey%22%5D)%3B%0A).

* [falsyBouncer](https://www.freecodecamp.com/challenges/Falsy%20Bouncer?solution=%0Afunction%20bouncer(arr)%20%7B%0A%20%20%2F%2F%20Don%27t%20show%20a%20false%20ID%20to%20this%20bouncer.%0A%20%20return%20arr.filter(function(val)%20%7B%0A%20%20%20%20return%20!!val%3B%0A%20%20%7D)%3B%0A%7D%0A%0Abouncer(%5B7%2C%20%22ate%22%2C%20%22%22%2C%20false%2C%209%5D)%3B%0A).

* [seekAndDestroy](https://www.freecodecamp.com/challenges/Seek%20and%20Destroy?solution=%0Afunction%20destroyer(arr)%20%7B%0A%20%20%2F%2F%20Remove%20all%20the%20values%0A%20%20var%20args%20%3D%20Array.prototype.slice.call(arguments)%3B%0A%20%20return%20arr.filter(function(element)%20%7B%0A%20%20%20%20return%20args.indexOf(element)%20%3E%20-1%20%3F%20%27%27%20%3A%20element%3B%0A%20%20%7D)%3B%0A%7D%0A%0Adestroyer(%5B1%2C%202%2C%203%2C%201%2C%202%2C%203%5D%2C%202%2C%203)%3B%0A).

* [whereDoIBelong](https://www.freecodecamp.com/challenges/Where%20do%20I%20belong?solution=%0Afunction%20getIndexToIns(arr%2C%20num)%20%7B%0A%20%20%2F%2F%20Find%20my%20place%20in%20this%20sorted%20array.%0A%20%20arr.sort(function(a%2C%20b)%20%7B%0A%20%20%20%20return%20(a%20-%20b)%3B%0A%20%20%7D)%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%3D%20arr.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(num%20%3C%3D%20arr%5Bi%5D)%20%7B%0A%20%20%20%20%20%20return%20i%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20arr.length%3B%0A%7D%0A%0AgetIndexToIns(%5B40%2C%2060%5D%2C%2050)%3B%0A).

* [caesarsCipher](https://www.freecodecamp.com/challenges/caesars-cipher#?solution=%0Afunction%20rot13(str)%20%7B%20%2F%2F%20LBH%20QVQ%20VG!%0A%20%20var%20char%20%3D%20''%3B%0A%20%20var%20decryptedStr%20%3D%20''%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%3D%20str.length%20-%201%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(str%5Bi%5D)%20%7B%0A%20%20%20%20%20%20var%20charCode%20%3D%20str.charCodeAt(i)%3B%0A%20%20%20%20%20%20if%20((charCode%20%3E%3D%2065)%20%26%26%20(charCode%20%3C%3D%2090))%20%7B%0A%20%20%20%20%20%20%20%20char%20%3D%20String.fromCharCode(((charCode%20-%2065%20%2B%2013)%20%25%2026)%20%2B%2065)%3B%0A%20%20%20%20%20%20%7D%20else%20if%20((charCode%20%3E%3D%2097)%20%26%26%20(charCode%20%3C%3D%20122))%20%7B%0A%20%20%20%20%20%20%20%20char%20%3D%20String.fromCharCode(((charCode%20-%2097%20%2B%2013)%20%25%2026)%20%2B%2097)%3B%0A%20%20%20%20%20%20%7D%20else%20if%20(charCode)%20%7B%0A%20%20%20%20%20%20%20%20char%20%3D%20String.fromCharCode(charCode)%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20decryptedStr%20%2B%3D%20char%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20decryptedStr%3B%0A%7D%0A%0A%2F%2F%20Change%20the%20inputs%20below%20to%20test%0Arot13(%22SERR%20PBQR%20PNZC%22)%3B%0A).

* [sumAllNumbersInRange](https://www.freecodecamp.com/challenges/sum-all-numbers-in-a-range#?solution=%0Afunction%20sumAll(arr)%20%7B%0A%20%20var%20arrSeq%20%3D%20%5B%5D%3B%0A%20%20for(var%20i%20%3D%20Math.min.apply(null%2C%20arr)%3B%20i%20%3C%3D%20Math.max.apply(null%2C%20arr)%3B%20i%2B%2B)%7B%0A%20%20%20%20arrSeq.push(i)%3B%0A%20%20%7D%0A%20%20return%20arrSeq.reduce(function(acc%2C%20pre)%7B%0A%20%20%20%20return%20acc%20%2B%20pre%3B%0A%20%20%7D%2C%200)%3B%0A%7D%0A%0AsumAll(%5B1%2C%204%5D)%3B%0A).

* [diffTwoArrays](https://www.freecodecamp.com/challenges/Diff%20Two%20Arrays?solution=%0Afunction%20diffArray(arr1%2C%20arr2)%20%7B%0A%20%20var%20newArr%20%3D%20%5B%5D%3B%0A%20%20%2F%2F%20Same%2C%20same%3B%20but%20different.%0A%20%20var%20firstArray%2C%20secondArray%3B%0A%20%20if%20(arr1.length%20%3E%3D%20arr2.length)%20%7B%0A%20%20%20%20firstArray%20%3D%20arr1%3B%0A%20%20%20%20secondArray%20%3D%20arr2%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20firstArray%20%3D%20arr2%3B%0A%20%20%20%20secondArray%20%3D%20arr1%3B%0A%20%20%7D%0A%20%20var%20firstArrayResult%20%3D%20firstArray.filter(function(first)%20%7B%0A%20%20%20%20return%20secondArray.indexOf(first)%20%3C%200%20%3F%20first%20%3A%20%27%27%3B%0A%20%20%7D)%3B%0A%20%20var%20secondArrayResult%20%3D%20secondArray.filter(function(second)%20%7B%0A%20%20%20%20return%20firstArray.indexOf(second)%20%3C%200%20%3F%20second%20%3A%20%27%27%3B%0A%20%20%7D)%3B%0A%20%20return%20newArr.concat(firstArrayResult%2C%20secondArrayResult)%3B%0A%7D%0A%0AdiffArray(%5B1%2C%202%2C%203%2C%205%5D%2C%20%5B1%2C%202%2C%203%2C%204%2C%205%5D)%3B%0A).

* [romanNumeralConverter ](https://www.freecodecamp.com/challenges/Roman%20Numeral%20Converter?solution=%0Afunction%20convertToRoman(num)%20%7B%0A%20%20decToRoman%20%3D%20%22%22%3B%0A%20%20romanNumericals%20%3D%20%5B%27M%27%2C%20%27CM%27%2C%20%27D%27%2C%20%27CD%27%2C%20%27C%27%2C%20%27XC%27%2C%20%27L%27%2C%20%27XL%27%2C%20%27X%27%2C%20%27IX%27%2C%20%27V%27%2C%20%27IV%27%2C%20%27I%27%5D%3B%0A%20%20decimalNumericals%20%3D%20%5B1000%2C%20900%2C%20500%2C%20400%2C%20100%2C%2090%2C%2050%2C%2040%2C%2010%2C%209%2C%205%2C%204%2C%201%5D%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%20romanNumericals.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20while%20(num%20%3E%3D%20decimalNumericals%5Bi%5D)%20%7B%0A%20%20%20%20%20%20decToRoman%20%2B%3D%20romanNumericals%5Bi%5D%3B%0A%20%20%20%20%20%20num%20-%3D%20decimalNumericals%5Bi%5D%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20decToRoman%3B%0A%7D%0A%0AconvertToRoman(36)%3B%0A).

* [whereforeArtThou](https://www.freecodecamp.com/challenges/wherefore-art-thou#?solution=%0Afunction%20whatIsInAName(collection%2C%20source)%20%7B%0A%20%20%2F%2F%20What's%20in%20a%20name%3F%0A%20%20var%20arr%20%3D%20%5B%5D%3B%0A%20%20%2F%2F%20Only%20change%20code%20below%20this%20line%0A%20%20arr%20%3D%20collection.filter(function(obj)%20%7B%0A%20%20%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%20Object.keys(source).length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20%20%20if%20(!obj.hasOwnProperty(Object.keys(source)%5Bi%5D)%20%7C%7C%20obj%5BObject.keys(source)%5Bi%5D%5D%20!%3D%3D%20source%5BObject.keys(source)%5Bi%5D%5D)%20%7B%0A%20%20%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20return%20true%3B%0A%20%20%7D)%3B%0A%20%20%2F%2F%20Only%20change%20code%20above%20this%20line%0A%20%20return%20arr%3B%0A%7D%0A%0AwhatIsInAName(%5B%7B%20first%3A%20%22Romeo%22%2C%20last%3A%20%22Montague%22%20%7D%2C%20%7B%20first%3A%20%22Mercutio%22%2C%20last%3A%20null%20%7D%2C%20%7B%20first%3A%20%22Tybalt%22%2C%20last%3A%20%22Capulet%22%20%7D%5D%2C%20%7B%20last%3A%20%22Capulet%22%20%7D)%3B%0A).

* [searchAndReplace](https://www.freecodecamp.com/challenges/search-and-replace#?solution=%0Afunction%20myReplace(str%2C%20before%2C%20after)%20%7B%0A%20%20var%20re%20%3D%20new%20RegExp(before%2C%20'gi')%3B%0A%20%20if%20(str.indexOf(before)%20%3E%200)%20%7B%0A%20%20%20%20if%20(%2F%5BA-Z%5D%2F.test(before%5B0%5D))%20%7B%0A%20%20%20%20%20%20after%20%3D%20after.charAt(0).toUpperCase()%20%2B%20after.slice(1)%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20str.replace(re%2C%20after)%3B%0A%7D%0A%0AmyReplace(%22A%20quick%20brown%20fox%20jumped%20over%20the%20lazy%20dog%22%2C%20%22jumped%22%2C%20%22leaped%22)%3B%0A).

* [pigLatin](https://www.freecodecamp.com/challenges/pig-latin#?solution=%0Afunction%20translatePigLatin(str)%20%7B%0A%20%20var%20regEx%20%3D%20(%2F%5E%5Baeiou%5D%24%2Fi)%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%3D%20str.length%20-%201%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(regEx.test(str%5B0%5D))%20%7B%0A%20%20%20%20%20%20return%20str%20%2B%20'way'%3B%0A%20%20%20%20%7D%20else%20if%20(regEx.test(str%5Bi%5D))%20%7B%0A%20%20%20%20%20%20return%20str.substring(i)%20%2B%20str.substring(0%2C%20i)%20%2B%20'ay'%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%7D%0A%0AtranslatePigLatin(%22consonant%22)%3B%0A).

* [dnaPairing](https://www.freecodecamp.com/challenges/dna-pairing#?solution=%0Afunction%20pairElement(str)%20%7B%0A%20%20var%20A%20%3D%20%5B'A'%2C%20'T'%5D%3B%0A%20%20var%20T%20%3D%20%5B'T'%2C%20'A'%5D%3B%0A%20%20var%20G%20%3D%20%5B'G'%2C%20'C'%5D%3B%0A%20%20var%20C%20%3D%20%5B'C'%2C%20'G'%5D%3B%0A%20%20var%20res%20%3D%20%5B%5D%3B%0A%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%3D%20str.length%20-%201%3B%20i%2B%2B)%20%7B%0A%20%20%20%20switch%20(str%5Bi%5D)%20%7B%0A%20%20%20%20%20%20case%20'A'%3A%0A%20%20%20%20%20%20%20%20res.push(A)%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20'T'%3A%0A%20%20%20%20%20%20%20%20res.push(T)%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20'G'%3A%0A%20%20%20%20%20%20%20%20res.push(G)%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20default%3A%0A%20%20%20%20%20%20%20%20res.push(C)%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20res%3B%0A%7D%0A%0ApairElement(%22GCG%22)%3B%0A).

* [missingLetters](https://www.freecodecamp.com/challenges/Missing%20letters?solution=%0Afunction%20fearNotLetter(str)%20%7B%0A%20%20if%20(%2F%5Ba-z%5D%2Fi.test(str))%20%7B%0A%20%20%20%20var%20i%20%3D%20str.charCodeAt(0)%3B%0A%20%20%20%20var%20j%20%3D%200%3B%0A%20%20%20%20while%20(i%20%3C%3D%20122%20%26%26%20j%20%3C%3D%20str.length%20-%201)%20%7B%0A%20%20%20%20%20%20if%20(String.fromCharCode(i)%20!%3D%3D%20str.charAt(j))%20%7B%0A%20%20%20%20%20%20%20%20return%20String.fromCharCode(i)%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20i%2B%2B%3B%0A%20%20%20%20%20%20j%2B%2B%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20undefined%3B%0A%7D%0A%0AfearNotLetter(%22abce%22)%3B%0A).

* [booWho](https://www.freecodecamp.com/challenges/Boo%20who?solution=%0Afunction%20booWho(bool)%20%7B%0A%20%20%2F%2F%20What%20is%20the%20new%20fad%20diet%20for%20ghost%20developers%3F%20The%20Boolean.%0A%20%20return%20typeof%20bool%20%3D%3D%3D%20%27boolean%27%20%3F%20true%20%3A%20false%3B%0A%7D%0A%0AbooWho(null)%3B%0A).

* [sortedUnion ](https://www.freecodecamp.com/challenges/Sorted%20Union?solution=%0Afunction%20uniteUnique(arr)%20%7B%0A%20%20var%20args%20%3D%20Array.prototype.slice.call(arguments)%3B%0A%20%20var%20res%20%3D%20args%5B0%5D%3B%0A%20%20args.map(function(val)%20%7B%0A%20%20%20%20val.reduce(function(accumulator%2C%20currentValue%2C%20currentIndex%2C%20array)%20%7B%0A%20%20%20%20%20%20return%20array.map(function(val)%20%7B%0A%20%20%20%20%20%20%20%20if%20(res.indexOf(val)%20%3C%200)%20%7B%0A%20%20%20%20%20%20%20%20%20%20res.push(val)%3B%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%7D)%3B%0A%20%20%20%20%7D)%3B%0A%20%20%7D)%3B%0A%20%20return%20res%3B%0A%7D%0A%0AuniteUnique(%5B1%2C%203%2C%202%5D%2C%20%5B5%2C%202%2C%201%2C%204%5D%2C%20%5B2%2C%201%5D)%3B%0A).

* [convertHtmlEntities](https://www.freecodecamp.com/challenges/Convert%20HTML%20Entities?solution=%0Afunction%20convertHTML(str)%20%7B%0A%20%20%2F%2F%20%26colon%3B%26rpar%3B%0A%0A%20%20return%20str.split(%27%27).map(function(val)%20%7B%0A%20%20%20%20switch%20(val)%20%7B%0A%20%20%20%20%20%20case%20%27%3C%27%3A%0A%20%20%20%20%20%20%20%20val%20%3D%20%27%26lt%3B%27%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20%27%26%27%3A%0A%20%20%20%20%20%20%20%20val%20%3D%20%27%26amp%3B%27%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20%27%3E%27%3A%0A%20%20%20%20%20%20%20%20val%20%3D%20%27%26gt%3B%27%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20%27%22%27%3A%0A%20%20%20%20%20%20%20%20val%20%3D%20%27%26quot%3B%27%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20case%20%22%27%22%3A%0A%20%20%20%20%20%20%20%20val%20%3D%20%22%26apos%3B%22%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%7D%0A%20%20%20%20return%20val%3B%0A%20%20%7D).join(%27%27)%3B%0A%7D%0A%0AconvertHTML(%22Dolce%20%26%20Gabbana%22)%3B%0A).

* [spinalTapCase](https://www.freecodecamp.com/challenges/Spinal%20Tap%20Case?solution=%0Afunction%20spinalCase(str)%20%7B%0A%20%20%2F%2F%20%22It%27s%20such%20a%20fine%20line%20between%20stupid%2C%20and%20clever.%22%0A%20%20%2F%2F%20--David%20St.%20Hubbins%0A%20%20str%20%3D%20str.replace(%2F(%5Ba-z%5D)(%5BA-Z%5D)%2Fg%2C%20%27%241%20%242%27)%3B%0A%20%20return%20str.toLowerCase().replace(%2F%5Cs%2B%7C_%2B%2Fg%2C%20%27-%27)%3B%0A%7D%0A%0AspinalCase(%27This%20Is%20Spinal%20Tap%27)%3B%0A).

* [sumAllOddFibonacciNumbers](https://www.freecodecamp.com/challenges/Sum%20All%20Odd%20Fibonacci%20Numbers?solution=%0Afunction%20sumFibs(num)%20%7B%0A%20%20var%20prev%20%3D%200%3B%0A%20%20var%20curr%20%3D%201%3B%0A%20%20var%20temp%20%3D%200%3B%0A%20%20var%20result%20%3D%200%3B%0A%20%20if%20(num%20%3D%3D%3D%201)%20%7B%0A%20%20%20%20result%20%3D%201%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20while%20(temp%20%3C%3D%20num)%20%7B%0A%20%20%20%20%20%20if%20(curr%20%25%202%20%3D%3D%3D%201)%20%7B%0A%20%20%20%20%20%20%20%20result%20%2B%3D%20curr%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20temp%20%3D%20curr%20%2B%20prev%3B%0A%20%20%20%20%20%20prev%20%3D%20curr%3B%0A%20%20%20%20%20%20curr%20%3D%20temp%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20result%3B%0A%7D%0A%0AsumFibs(4)%3B%0A).

* [sumAllPrimes](https://www.freecodecamp.com/challenges/Sum%20All%20Primes?solution=%0Afunction%20sumPrimes(num)%20%7B%0A%20%20var%20count%20%3D%200%3B%0A%20%20var%20res%20%3D%200%3B%0A%20%20var%20flag%3B%0A%20%20for%20(var%20i%20%3D%202%3B%20i%20%3C%3D%20num%3B%20i%2B%2B)%20%7B%0A%20%20%20%20flag%20%3D%20true%3B%0A%20%20%20%20for%20(var%20j%20%3D%202%3B%20j%20%3C%20i%3B%20j%2B%2B)%20%7B%0A%20%20%20%20%20%20if%20(i%20%25%20j%20%3D%3D%3D%200)%20%7B%0A%20%20%20%20%20%20%20%20flag%20%3D%20false%3B%0A%20%20%20%20%20%20%20%20break%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20if%20(flag)%20%7B%0A%20%20%20%20%20%20res%20%2B%3D%20i%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20res%3B%0A%7D%0A%0AsumPrimes(10)%3B%0A).

* [smallestCommonMultiple](https://www.freecodecamp.com/challenges/Smallest%20Common%20Multiple?solution=%0Afunction%20smallestCommons(arr)%20%7B%0A%20%20var%20startVal%20%3D%20Math.min.apply(null%2C%20arr)%3B%0A%20%20var%20endVal%20%3D%20Math.max.apply(null%2C%20arr)%3B%0A%20%20var%20findLcmForArr%20%3D%20%5B%5D%3B%0A%0A%20%20for%20(var%20i%20%3D%20startVal%3B%20i%20%3C%3D%20endVal%3B%20i%2B%2B)%20%7B%0A%20%20%20%20findLcmForArr.push(i)%0A%20%20%7D%0A%0A%20%20function%20gcd(a%2C%20b)%20%7B%0A%20%20%20%20return%20!b%20%3F%20a%20%3A%20gcd(b%2C%20a%20%25%20b)%3B%0A%20%20%7D%0A%0A%20%20function%20lcm(a%2C%20b)%20%7B%0A%20%20%20%20return%20(a%20*%20b)%20%2F%20gcd(a%2C%20b)%3B%0A%20%20%7D%0A%0A%20%20var%20multiple%20%3D%20startVal%3B%0A%20%20findLcmForArr.map(function(n)%20%7B%0A%20%20%20%20multiple%20%3D%20lcm(multiple%2C%20n)%3B%0A%20%20%20%20return%20multiple%3B%0A%20%20%7D)%3B%0A%20%20return%20multiple%3B%0A%7D%0A%0A%0AsmallestCommons(%5B1%2C5%5D)%3B%0A).

* [findersKeepers ](https://www.freecodecamp.com/challenges/finders-keepers#?solution=%0Afunction%20findElement(arr%2C%20func)%20%7B%0A%20%20var%20num%20%3D%20%5B%5D%3B%0A%0A%20%20arr.filter(function(val)%20%7B%0A%20%20%20%20if%20(func(val))%20%7B%0A%20%20%20%20%20%20num.push(val)%3B%0A%20%20%20%20%7D%0A%20%20%7D)%3B%0A%20%20return%20num%5B0%5D%3B%0A%7D%0A%0AfindElement(%5B1%2C%202%2C%203%2C%204%5D%2C%20function(num)%7B%20return%20num%20%25%202%20%3D%3D%3D%200%3B%20%7D)%3B%0A).

* [dropIt ](https://www.freecodecamp.com/challenges/Drop%20it?solution=%0Afunction%20dropElements(arr%2C%20func)%20%7B%0A%20%20%2F%2F%20Drop%20them%20elements.%0A%20%20var%20res%20%3D%20%5B%5D%3B%0A%20%20arr.findIndex(function(val)%20%7B%0A%20%20%20%20if%20(func(arr%5B0%5D))%20%7B%0A%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20arr.shift()%3B%0A%20%20%20%20%7D%0A%20%20%7D)%3B%0A%20%20return%20arr%3B%0A%7D%0A%0AdropElements(%5B1%2C%202%2C%203%5D%2C%20function(n)%20%7Breturn%20n%20%3C%203%3B%20%7D)%3B%0A).

* [steamroller](https://www.freecodecamp.com/challenges/Steamroller?solution=%0Afunction%20steamrollArray(arr)%20%7B%0A%20%20%2F%2F%20I%27m%20a%20steamroller%2C%20baby%0A%20%20return%20arr.reduce(function(prev%2C%20curr)%20%7B%0A%20%20%20%20return%20prev.concat(Array.isArray(curr)%20%3F%20steamrollArray(curr)%20%3A%20curr)%3B%0A%20%20%7D%2C%20%5B%5D)%3B%0A%7D%0A%0AsteamrollArray(%5B1%2C%20%5B2%5D%2C%20%5B3%2C%20%5B%5B4%5D%5D%5D%5D)%3B%0A).

* [binaryAgents](https://www.freecodecamp.com/challenges/Binary%20Agents?solution=%0Afunction%20binaryAgent(str)%20%7B%0A%20%20return%20str.split(%27%20%27).map(function(val)%7B%0A%20%20%20%20%20%20return%20String.fromCharCode(parseInt(val%2C2).toString(10))%3B%0A%20%20%7D).join(%27%27)%3B%0A%7D%0A%0AbinaryAgent(%2201000001%2001110010%2001100101%2001101110%2000100111%2001110100%2000100000%2001100010%2001101111%2001101110%2001100110%2001101001%2001110010%2001100101%2001110011%2000100000%2001100110%2001110101%2001101110%2000100001%2000111111%22)%3B%0A).

For more details please visit [My Free Code Camp Profile](https://www.freecodecamp.com/aadhikar).

<!-- 
* [link](url).
  -->
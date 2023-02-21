 1. Count number of words in a Text after splitting it by any word
       for example
         Hello Wecode Acacdemy
         space se split, 3 words

      ```
          let str = "Hello Wecode Acacdemy";
          let split = str.split("Wecode");
          console.log(split.length);
      ```

      2. Convert odd position word to lowercase and even position word to uppercase
         foe example
       Hello WeCode Academy
       hello WECODE academy
      for example
      ```
        let str = "Hello WeCode Academy my name Is Farman Khan";
        let split = str.split(" ");
        let empty = "";
        for (let x = 0; x < split.length; x++) {
          if (x % 2 === 1) {
            empty += " " + split[x].toLowerCase();
          } else if (x % 2 === 0) {
            if (x === 0) {
              empty += split[x].toUpperCase();
            } else {
              empty += " " + split[x].toUpperCase();
            }
          }
        }
        console.log(empty);
      ```//for example //   3. Capitalize each word of the string

      ```
      //   hello wecode academy jhotwara jaipur
      //   Hello Wecode Academy Jhotwara Jaipur
        let str = "hello wecode academy jhotwara jaipur";
        let empty = "";
        let split = str.split(" ");
        for (let x = 0; x < split.length; x++) {
          if (split[x] == split[split.length - 1]) {
            let a = split[x].slice(0, 1).toUpperCase();
            let b = split[x].slice(1).toLowerCase();
            let c = a.concat(b);
            empty += c;
          } else {
            let a = split[x].slice(0, 1).toUpperCase();
            let b = split[x].slice(1).toLowerCase();
            let c = a.concat(b);
            empty += c + " ";
          }
        }
        console.log(empty);
        ```//for example //4. Convert an string into 2 halfs and change the position of the other half
      ```
         My name is wecode academy
         wecode academy My name is
        let str = "My name is wecode academy";
        let split = str.split(" ");
        let slice1 = split.slice(0, Math.ceil(split.length / 2));
        let slice2 = split.slice(Math.ceil(split.length / 2));
        let concat = slice2.concat(slice1);
        let join = concat.join(" ");
        console.log(join);
        ```;

      //5. Take a string and now ask for a character from the user. Now find total count of that character in the string
      //for example
      // My name is wecode academy;
      // a
      // 3
      ```
      let str = "My name is wecode academy";
      let ask = prompt("what do you wnt to find in string?");
      let split = str.split(" ");
      let count = 0;
      for (let x = 0; x < split.length; x++) {
        if (split[x].includes(ask)) {
          count += 1;
        }
      }
      console.log(count);
      ```//6. Reverse a string
      ```
        let str = "my name is farman khan";
        let split = str.split(" ").reverse();
        let empty = "";
        for (let x = 0; x < split.length; x++) {
          let a = split[x].split("").reverse().join("");
          empty += a + " ";
        }
        console.log(empty);
        ```//7. Check string is palindrom or not
      ```
        let str = "abababa";
        let split = str.split(" ");
        let empty = "";
        for (let x = 0; x < split.length; x++) {
          let a = split[x].split("").reverse().join("");
          if (x === 0) {
            empty += a;
          } else {
            empty += a + " ";
          }
        }
        if (empty === str) {
          console.log("yes");
        } else {
          console.log("no");
        }
        ```//8. Remove space from the string and show the output
      //for example
      ```
        My name is wecode
        Mynameiswecode
        let str = "My name is wecode";
        let split = str.split(" ");
        let empty = "";
        for (let x = 0; x < split.length; x++) {
          b = split[x];
          empty += b;
        }
        console.log(empty);
        ```//   9. Check a word count in the string
      //   for exemple
      //   My code is wecode and wecode Jhotwara, Jaipur.
      //   code
      //   3
      ```
        let str = "My code is wecode and wecode Jhotwara, Jaipur.";
        let ask = prompt("what do you want to serch?");
        let split = str.split(" ");
        let count = 0;
        for (let x = 0; x < split.length; x++) {
          if (split[x].includes(ask)) {
            count += 1;
          }
        }
        console.log(count);
        ```;

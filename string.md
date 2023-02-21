     ```
     1. Count number of words in a Text after splitting it by any word dalfirw egiegt e
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

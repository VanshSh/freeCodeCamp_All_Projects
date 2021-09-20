<h1 align="center">freeCodeCamp Projects</h1>

<h2 align= "center">:loudspeaker: Responsive Web Design :loudspeaker:</h2>

1. ## Build a Tribute Page
     :link: Repository [Link](https://github.com/VanshSh/Tribute-Page-FreeCodeCamp)
    
     :tv:   Live [Demo](https://codepen.io/vanshsh/full/bGqLgzM) 

1. ## Build a Survey Form
     :link: Repository [Link](https://github.com/VanshSh/Survey-Form-FreeCodeCamp)
    
     :tv:   Live [Demo](https://codepen.io/vanshsh/full/GRWdjXy)

1. ## Build a Product Landing Page
     :link: Repository [Link](https://github.com/VanshSh/Landing-Page-FreeCodeCamp)
    
     :tv:   Live [Demo](https://codepen.io/vanshsh/full/bGqLgzM)

1. ## Build a Technical Documentation Page
     :link: Repository [Link](https://github.com/VanshSh/HTML-Form-Documentation-FreeCodeCamp)
    
     :tv:   Live [Demo](https://codepen.io/vanshsh/full/MWpRKWP) 

1. ## Build a Personal Portfolio Webpage
     :link: Repository [Link](https://github.com/VanshSh/Portfolio-FreeCodeCamp)
    
     :tv:   Soon 


## :mortar_board: [Certificate](https://www.freecodecamp.org/certification/vanshsharma2701/responsive-web-design)

***

<h2 align= "center">:loudspeaker: JavaScript Algorithms and Data Structures :loudspeaker:</h2>

1. ## Palindrome Checker 

     ### :tv:  Live [Demo](https://codepen.io/vanshsh/full/xxrpZaR) 


1. ## Roman Numeral Converter

     ### :tv:  Live [Demo](https://codepen.io/vanshsh/full/mdwXVzB) 



1. ## Caesars Cipher

     ### :tv:  Live [Demo](https://codepen.io/vanshsh/full/abwYobd) 


1. ## Telephone Number Validator

     ### :tv:  Live [Demo](https://codepen.io/vanshsh/full/JjJLOQw) 


1. ## Cash Register

:desktop_computer:
<details>

    ```

     const checkCashRegister = (price, cash, cid) => {
     
     const UNIT_AMOUNT = {
    "PENNY": .01,
    "NICKEL": .05,
    "DIME": .10,
    "QUARTER": .25,
    "ONE": 1.00,
    "FIVE": 5.00,
    "TEN": 10.00,
    "TWENTY": 20.00,
    "ONE HUNDRED": 100.00
     }
     let totalCID = 0;
     for (let element of cid) {
     totalCID += element[1];
     }
     totalCID = totalCID.toFixed(2);
     let changeToGive = cash - price;
     const changeArray = [];
     if (changeToGive > totalCID) {
      return { status: "INSUFFICIENT_FUNDS", change: changeArray };
     } else if (changeToGive.toFixed(2) === totalCID) {
     return { status: "CLOSED", change: cid };
     }   else {
     cid = cid.reverse();
     for (let elem of cid) {
      let temp = [elem[0], 0];
      while (changeToGive >= UNIT_AMOUNT[elem[0]] && elem[1] > 0) {
        temp[1] += UNIT_AMOUNT[elem[0]];
        elem[1] -= UNIT_AMOUNT[elem[0]];
        changeToGive -= UNIT_AMOUNT[elem[0]];
        changeToGive = changeToGive.toFixed(2);
      }
      if (temp[1] > 0) {
        changeArray.push(temp);
      }
    }
       }
    if (changeToGive > 0) {
    return { status: "INSUFFICIENT_FUNDS", change: [] };
     }
     return { status: "OPEN", change: changeArray};
     }

    ```

</details>

## :mortar_board: [Certificate](https://www.freecodecamp.org/certification/vanshsharma2701/javascript-algorithms-and-data-structures)

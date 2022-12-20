# Dom Manipulation Assignment

### Topics

    - Query Selector, Inner HTML


1. Website Name: [Dev To](https://dev.to/)

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output


![Output](./Pic2.png)

### Solution
```javascript
document.querySelector(".sidebar-wrapper .lh-tight").innerHTML = "iNeuron"
document.querySelector(".sidebar-wrapper .crayons-card .color-base-70").innerHTML = "I Write Code"
```

2. Website Name: [Apple](https://support.apple.com/en-in)

### Sample Image

![Store](./Picture_3.png)

### Task

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

### Solution
```javascript
let grabElement = document.querySelectorAll(".as-imagegrid-item-title")
fetchData = [];
for(let i=0; i<=grabElement.length; i++){fetchData.push(grabElement[i].innerHTML.split(" ")[0])}
```

3. Website Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

### Solution

```javascript
let grabElement = document.querySelector(".accordion-homepage");
newFaqSection = document.createElement('section');
myNewFaq = document.createElement('h3');
myNewFaq.innerText = "My New FAQ"
newFaqSection.appendChild(myNewFaq);
grabElement.appendChild(newFaqSection);
newFaqSection.className = "parent";
```

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

### Solution
```javascript
document.querySelector(".item--subtitle").innerHTML = "6366256689"
```
5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)

### Solution

```javascript
let samsungBtn = document.querySelectorAll(".diwali-deals-product-sale-btn")[30]
samsungBtn.innerText = "Check Out"
```

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)

### Solution

```javascript
let icon = document.querySelector(".searchinput___19uW0");
icon.addEventListener('mouseenter',()=>{icon2.style.backgroundColor = "red"});
icon.addEventListener('mouseout',()=>{icon2.style.backgroundColor = "none"});
```

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

### Solution
```javascript
document.querySelector(".search-input-field").value = "CSS Selectors"
document.querySelector("#top-nav-search-form").submit();
```

8. Website Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

### Solution
```javascript
languageRemover = document.querySelector("#SIvCob").childNodes
for(let i = languageRemover.length-2; i>1; i=i-4){languageRemover[i].remove()}
```

9. Website Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

### Solution
```javascript
document.querySelector(".text-color-white").style.color = "#b03d3d"
document.querySelector(".text-color-white").style.fontFamily = "Monospace"
```

10. Website Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

### Solution

```javascript
let getStarted = document.querySelectorAll(".login-btn-text")[1];
trial.addEventListener('mouseenter',()=>{trial.style.backgroundColor = "red"});
trial.addEventListener('mouseout',()=>{trial.style.backgroundColor = "transparent"});
```

11. Website Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

### Solution

```javascript
document.querySelector(".icon-logo").style.backgroundImage = "URL('https://learn.ineuron.ai/_next/image?url=%2Fimages%2Fineuron-logo.png&w=1920&q=75')"
```

12. Website Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

### Solution

```javascript
document.querySelectorAll(".btn-primary")[1].style.backgroundColor = "blue"
```

13. Website Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

### Solution
```javascript
let hackerRank = document.querySelector(".home22-intro-text").childNodes[0].innerHTML = "JS Bootcamp"
```

14. Website Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

### Solution

```javascript
document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "80px"
```
15. Website Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

```javascript
let g15 = document.querySelectorAll(".ps-top")[4];
g15.querySelector(".ps-title").style.textAlign = "right"
```

16. Website Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)

### Solution

```javascript
document.querySelector(".section-title_title__VEDfK").innerHTML = "Start with scratch"
```
17. Website Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)

### Solution

```javascript
let sonyBtn = document.querySelector(".btn-container");
let now = new Date();
sonyBtn.innerHTML = now.toString();
```

18. Website Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

### Solution

```javascript
document.querySelector(".p-footer").style.backgroundColor = "orange"
```

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

### Solution

```javascript
console.log(document.querySelector(".navbar-brand").childNodes[1].currentSrc);
```

20. Website Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

### Solution

```javascript
document.querySelectorAll(".desc")[3].style.color = "orange"
```
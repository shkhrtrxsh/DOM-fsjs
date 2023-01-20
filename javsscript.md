# Dom Manipulation Assignment

1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)
//Answer 
document.querySelector(".crayons-subtitle-2")
<h2 class=​"crayons-subtitle-2 lh-tight mb-4">​ DEV Community 👩&zwj;💻👨&zwj;💻 is a community of 993,399 amazing developers ​</h2>​
document.querySelector(".crayons-subtitle-2").innerText="Ineuron";
'Ineuron'
document.querySelector(".color-base-70");
<p class=​"color-base-70 mb-4">​…​</p>​
document.querySelector(".color-base-70").innerText="i write code.";
'i write code.'


2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

//ans
var arr=document.querySelectorAll(".as-imagegrid-item");
arr.forEach(function(element){
    var productName=element.querySelector("a").getAttribute("data-analytics-link-component_name");
    productNames.push(productName);})
console.log(productNames);

3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)
//ans
var originalElement=document.querySelectorAll(".parent")[0];
var newElement=document.createElement("section");
let attributes = originalElement.attributes;
for (let i = 0; i < attributes.length; i++) {
    newElement.setAttribute(attributes[i].name, attributes[i].value);
};
newElement.innerHTML = originalElement.innerHTML;
var insidee=newElement.querySelector("h3");
insidee.innerText="My New FAQ";
var parent=document.querySelector(".accordion-homepage");
parent.appendChild(newElement);

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)
//ANS
var parent=document.querySelectorAll(".listing")[2];
var inside=parent.querySelectorAll(".mytabs")[2];
var insidee=inside.querySelector("div");
insidee.querySelectorAll("a")[1].innerText="checkout";


6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)
//ans
document.querySelector("._input_1f3oz_13").addEventListener("mouseover",(event)=>{ event.target.style.backgroundColor="red"});
document.querySelector("._input_1f3oz_13").addEventListener("mouseout",(event)=>{ event.target.style.backgroundColor=""});

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)
document.getElementById("hp-search-input").value="CSS Selectors";
document.getElementById("hp-search-form").submit();

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)
var items=document.querySelectorAll("a");
for(var i=5;i<14;i++){
    if(i%2==0){
        items[i].remove();
    }};
9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)
//ans
document.querySelector(".text-color-white");
<h1 class=​"text-color-white">​…​</h1>​
var div=document.querySelector(".text-color-white");
undefined
div.style.fontFamily="monospace";
'monospace'
div.style.color="red";
'red'
document.querySelector(".text-color-hero-gradient").style.color="red";
'red'


10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)
//ans
var div=document.querySelectorAll(".login-btn-text")[1];
undefined
div.addEventListener("mouseover",(event)=>{ event.target.style.backgroundColor="red"});


11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)
//Ans
var item=div.querySelector("span");
item.style.backgroundImage = "url('https://ineuron.ai/images/ineuron-logo.png')";x`

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)
//ans
var div=document.querySelector(".f4");
var inside=div.querySelector("a");
inside.style.backgroundColor="blue";

13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)
//ans
var div=document.querySelector(".HotDealsAll__Heading__2fIbe");
div.style.fontSize="80px";

15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)
//ans
var div=document.querySelectorAll(".ps-title")[4];
div.style.textAlign="right";

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)
//ans
var inside=document.querySelectorAll(".section-title_title__VEDfK")[0];
inside.innerText="Start with Scratch";

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)
//ans
var div=document.querySelectorAll(".btn-container")[0];
var today = new Date();
div.innerHTML="<h1>Today's date is: " + today.toLocaleDateString() + "</h1>";

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)
//ans
var div=document.querySelector(".p-f03-footer-container ");
div.style.background="yellow";

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)
//ans
var div=document.querySelector(".logo");
var inside=location.origin + div.getAttribute("src");

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)
//ANS
var div=document.querySelector(".desc");
div.style.color="orange";

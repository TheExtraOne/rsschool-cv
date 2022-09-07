# Kate Mikhasiova
### Junior Frontend Developer
---------------------
### Contacts:
Phone: +375 29 630 44 37

E-mail: katya_mihasewa@mail.ru

Telegram: @The_Extra_one

Discord: TheExtraOne

---------------------
### About myself:
I’m a 25-years old person with relatively rich backgrounds, as I used to work as a surgeon in a State Institution "Minsk Scientific and Practical Center for Surgery, Transplantology and Hematology". 
My hard decision to leave medicine was a turning point, but I was totally obsessed by programming, so chose to be a risk taker — and thereby hangs a tale.
After completing "Basics of Computed Science" course, I acquired not only new skills, but also a sense of moving in the right direction and discovered a great ability to learn. 
Literally, it was like a breath of fresh air for me, so my next step was to cope with "Website development with HTML, CSS and base JS" course in the it-academy. It was gripping to investigate something new, to deal with obstacles and challenges, to think outside the box and finally create my own first website (you can find a link below). 
Now I’m working hard at finishing "JavaScript web application development course" and thinking about advantages of The Rolling Scopes School experience.

My strong qualities: motivated and assertive, reliable, equally mastered soft skills (thanks to medicine), a team worker, can easily prioritize tasks (+multitasking), punctual (trying to do things in advance) and can cope with failure.
It is a real challenge to wind me up. 
And I’m also a woman of integrity who has never abandoned her principles for the sake of making money and always kept up my end of the deal.

As I want to put the finishing touches to this part of my CV, I should simply add, that focusing only on work is a bit destructive and unproductive, so I have a good work-life balance. For e.g. travelling helps to recharge my batteries and numerous hobbies make me feel refreshed.

------------------
### Skills and abilities:
* HTML, CSS
* JavaScript
* SASS
* Bootstrap, Foundation, Materialize, JQuery
* Git, GitHub
* Visual Studio Code
* Methodologies: BEM
-------------------
### Code example:
```'use strict'

class HashStorageFunc {
  constructor() {
    this.items = {};
  }
  addValue(key, value) {					
    this.items[key] = value;
  }
  getValue(key) {
    return this.items[key];
  }
  deleteValue(key) {
    if (key in this.items) {
      delete this.items[key];
      return true;
    } else {
      return false;
    }
  }
  getKeys() {
    return Object.keys(this.items);
  }
}

let drinkStorage = new HashStorageFunc();

let addUserInfoButton = document.querySelector('.addUserInfoButton');
addUserInfoButton.addEventListener('click', addUserInfo, false);

let getDrinkInfoButton = document.querySelector('.getDrinkInfoButton');
getDrinkInfoButton.addEventListener('click', getDrinkInfo, false);

let deleteDrinkInfoButton = document.querySelector('.deleteDrinkInfoButton');
deleteDrinkInfoButton.addEventListener('click', deleteDrinkInfo, false);

let userDrinksListButton = document.querySelector('.userDrinksListButton');
userDrinksListButton.addEventListener('click', userDrinksList, false);

function addUserInfo() {  
  let drinkName = prompt('Введите название напитка');
  let containAlc = confirm('Если напиток алкогольный, нажмите "ОК", если нет - то "Отмена"') ? 'да' : 'нет';
  let drinkRecipe = prompt('Ведите рецепт напитка');

  drinkStorage.addValue( drinkName, {'alco' : containAlc, 'recipe' : drinkRecipe,} );
}

function getDrinkInfo() {   
  let drinkName = prompt('Введите название напитка');
  let result = drinkStorage.getValue(drinkName);

  (result) ? alert('напиток ' + drinkName + '\n алкогольный: ' + result.alco + '\n рецепт приготовления: ' + result.recipe) : alert('Такого напитка в хранилище нет');
}

function deleteDrinkInfo() {  
  let drinkName = prompt('Введите название напитка');
  let result = drinkStorage.deleteValue(drinkName);
  
  (result) ? alert('Рецепт удалён') : alert('Такого напитка в хранилище нет');
}

function userDrinksList() {
  return alert(drinkStorage.getKeys());
}
```
-------------------
### Education and experience:
* Basics of Computed Science (it-academy)
* Website development with HTML, CSS and base JS (it-academy)
* JavaScript web application development course (it-academy, in progress)
* RS Schools Course «JavaScript/Front-end. Stage 1» (in progress)
* Belarussian State Medical University

Link to my final project ("Website development with HTML, CSS and base JS"): [Art School](https://theextraone.github.io/Final-Project/index.html)

-----------------------
### Languages:
* English B2 (Streamline certificate)
* German A1 (Streamline certificate)
* Russian (native)
* Belarussian (native)




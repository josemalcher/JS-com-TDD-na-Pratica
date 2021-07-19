# JS com TDD na Prática

https://www.udemy.com/course/js-com-tdd-na-pratica/

Aprenda testes na prática e garanta um currículo melhor para o mercado de trabalho.

## <a name="indice">Índice</a>

1. [Seção 1: Boas Práticas](#parte1)     
2. [Seção 2: Aprendendo ES6](#parte2)     
3. [Seção 3: Atualizações ES7/ES8](#parte3)     
4. [Seção 4: Módulos em JS](#parte4)     
5. [Seção 5: Teoria de Testes](#parte5)     
6. [Seção 6: Unindo conceitos na prática](#parte6)     
7. [Seção 7: Criando uma Biblioteca Wrapper da API do Spotify](#parte7)     
8. [Seção 8: Refatorando uma biblioteca com testes](#parte8)     
9. [Seção 9: Criando um Player do Spotify](#parte9)     
10. [Seção 10: Criando uma CLI para converter Bitcoin em qualquer moeda](#parte10)     
11. [Seção 11: Introdução a Testes com React - Criando um Componente Full Header](#parte11)     
---


## <a name="parte1">1 - Seção 1: Boas Práticas</a>

1. Introdução

- [https://github.com/willianjusten/js-tdd-course](https://github.com/willianjusten/js-tdd-course)
- [https://travis-ci.org/https://github.com/](https://travis-ci.org/https://github.com/)
- [https://github.com/](https://github.com/)
- [https://nodejs.org/en/](https://nodejs.org/en/)
- [https://git-scm.com/](https://git-scm.com/)
- [https://www.npmjs.com/](https://www.npmjs.com/)

2. Configurando o NPM e Criando o package.json

- [https://docs.npmjs.com/cli/v7/using-npm/config](https://docs.npmjs.com/cli/v7/using-npm/config)
- [https://docs.npmjs.com/](https://docs.npmjs.com/)
- [https://www.npmjs.com/](https://www.npmjs.com/)

```
$ npm -v
7.11.2

$ npm set init-author-name "José Malcher Jr."

$ npm set init-author-email "malcher.malch@gmail.com"

$ npm set init-author-url "https://josemalcher.net"

$ npm set init-license "MIT"

$ npm adduser
npm notice Log in on https://registry.npmjs.org/
Username: josemalcher
Password:
Email: (this IS public) malcher.malch@gmail.com
Logged in as josemalcher on https://registry.npmjs.org/.

```

3. Criando o gitignore de forma simples

- [https://www.npmjs.com/package/gitignore](https://www.npmjs.com/package/gitignore)

4. Criando arquivos para documentação

- [https://github.com/matiassingers/awesome-readme](https://github.com/matiassingers/awesome-readme)
- [https://github.com/lyef/lyef-react-component](https://github.com/lyef/lyef-react-component)
- [https://opensource.org/licenses](https://opensource.org/licenses)

5. Padrões de Código - Styleguides

- [https://github.com/airbnb/javascript](https://github.com/airbnb/javascript)
- [https://github.com/standard/standard](https://github.com/standard/standard)
- [https://github.com/rwaldron/idiomatic.js/](https://github.com/rwaldron/idiomatic.js/)
- [http://jscs.info/](http://jscs.info/)
- [https://eslint.org/](https://eslint.org/)


6. Instalando e Usando o Eslint

- [https://willianjusten.com.br/analisando-seu-codigo-js-com-linter/](https://willianjusten.com.br/analisando-seu-codigo-js-com-linter/)
- [https://www.jetbrains.com/help/phpstorm/eslint.html#ws_js_eslint_verify_code](https://www.jetbrains.com/help/phpstorm/eslint.html#ws_js_eslint_verify_code)
- [https://blog.cod3r.com.br/organizacao-e-padronizacao-com-eslint/](https://blog.cod3r.com.br/organizacao-e-padronizacao-com-eslint/)


7. UPDATE: Atualizando o Eslint para 4+

8. Configurando o editorconfig

- [https://editorconfig.org/](https://editorconfig.org/)
- [https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
- [https://plugins.jetbrains.com/plugin/7294-editorconfig/](https://plugins.jetbrains.com/plugin/7294-editorconfig/)

9. Criando um Npm Script

- [https://css-tricks.com/why-npm-scripts/](https://css-tricks.com/why-npm-scripts/)

10. Configurando hooks no git

- [https://github.com/typicode/husky](https://github.com/typicode/husky)
- [https://git-scm.com/book/it/v2/Customizing-Git-Git-Hooks](https://git-scm.com/book/it/v2/Customizing-Git-Git-Hooks)

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Seção 2: Aprendendo ES6</a>

11. 1 - Introdução ao ES6

- [https://nipher.io/](https://nipher.io/)
- [https://ponyfoo.com/articles/tagged/es6-in-depth](https://ponyfoo.com/articles/tagged/es6-in-depth)
- [http://kangax.github.io/compat-table/es6/](http://kangax.github.io/compat-table/es6/)
- [http://es6-features.org/#Constants](http://es6-features.org/#Constants)
- [https://github.com/willianjusten/es6-curso](https://github.com/willianjusten/es6-curso)

12. 2.1 - Escopo do JS

- [Secao-02-Aprendendo-ES6/21-Escopo-do-JS.html](Secao-02-Aprendendo-ES6/21-Escopo-do-JS.html)

```javascript
var animal;

function sayAnimal() {
    animal = 'cat';
    console.log(animal);
}

sayAnimal();

console.log(animal);

let sound = 'meow';
const name = 'jake';

```

13. 2.2 - Variável let no JS

- [Secao-02-Aprendendo-ES6/22-Variavel-let-no-JS.html](Secao-02-Aprendendo-ES6/22-Variavel-let-no-JS.html)

```javascript
    var animal = 'cat';
    console.log(animal); // cat

    {
        let animal = 'DOG';
        console.log(animal) // DOG
    }

    console.log(animal) // cat
```

14. 2.3 - Variável const no JS

- [Secao-02-Aprendendo-ES6/23-Variavel-const-no-JS.html](Secao-02-Aprendendo-ES6/23-Variavel-const-no-JS.html)

```javascript
    const secreteNumber = 20;

    const jose = {
        name: 'Jose Malcher jr',
        age: 36
    }
    Object.freeze(jose); // 'congela' o atributos do objeto

    jose.age = 10;

    console.log(jose)
```

15. 2.4 - Temporal Dead Zone

- [Secao-02-Aprendendo-ES6/24-Temporal-Dead-Zone.html](Secao-02-Aprendendo-ES6/24-Temporal-Dead-Zone.html)

```javascript
    console.log(dog);
    //let dog = 'GRRRRRRRR'; // Uncaught ReferenceError: Cannot access 'dog' before initialization
    const dog = 'GRRRRRRRR'; // Uncaught ReferenceError: Cannot access 'dog' before initialization

    //var dog = 'GRRRRRRRR'; // undefined
```

16. 3.1 - Introdução a Arrow Function

- [https://ponyfoo.com/articles/es6-arrow-functions-in-depth](https://ponyfoo.com/articles/es6-arrow-functions-in-depth)
- [https://nipher.io/ES6-arrow-functions/](https://nipher.io/ES6-arrow-functions/)

- [Secao-02-Aprendendo-ES6/31-Introducao-a-Arrow-Function.html(Secao-02-Aprendendo-ES6/31-Introducao-a-Arrow-Function.html)

```javascript
  const ireland = ['Dublin', 'Galway', 'Brasil'];

    const maps1 = ireland.map(function (name) {
        return `Eu amo ${name}!`;
    })
    console.log(maps1); //(3)["Eu amo Dublin!", "Eu amo Galway!", "Eu amo Brasil!"]

    const maps2 = ireland.map((name) => {
        return `Eu amo ${name}!`;
    })
    console.log(maps2); // (3)["Eu amo Dublin!", "Eu amo Galway!", "Eu amo Brasil!"]

    const maps3 = ireland.map(name => {
        return `Eu amo ${name}!`;
    })
    console.log(maps3); // (3)["Eu amo Dublin!", "Eu amo Galway!", "Eu amo Brasil!"]

    const maps4 = ireland.map(name => `Eu amo ${name}!`);

    console.log(maps4); // (3)["Eu amo Dublin!", "Eu amo Galway!", "Eu amo Brasil!"]

    const mapsfilter = ireland
        .filter(name => name === 'Brasil')
        .map(name => `Eu amo ${name}!`);

    console.log(mapsfilter); // ["Eu amo Brasil!"]
```

17. 3.2 - Arrow Function e o Lexical This

- [Secao-02-Aprendendo-ES6/32-Arrow-Function-e-o-Lexical-This.html](Secao-02-Aprendendo-ES6/32-Arrow-Function-e-o-Lexical-This.html)

```javascript
    const sandwich = {
        bread: 'white',
        cheese: 'cheedar',

        prepare: function () {
            return `I want a sandwich with ${this.bread} bread and ${this.cheese} cheese!`;
        },

        make: function () {
            window.setTimeout(
                () => {
                    console.log(this.prepare());
                }, 500)
        }
    };

    const btn = document.getElementById('btn');

    btn.addEventListener('click', function () {
        sandwich.make();
    });

```

18. 4.1 - Introdução a Template Literals

- [https://ponyfoo.com/articles/es6-template-strings-in-depth](https://ponyfoo.com/articles/es6-template-strings-in-depth)
- [https://nipher.io/es6-template-literals/](https://nipher.io/es6-template-literals/)
- [Secao-02-Aprendendo-ES6/41-Introducao-a-Template-Literals.html](Secao-02-Aprendendo-ES6/41-Introducao-a-Template-Literals.html)

```javascript
    const ireland = {
        live: 'Dublin',
        love: 'Galway'
    };

    const text = 'Eu moro em ' + ireland.live + ' e sou apaixonado por ' + ireland.love+'!';

    const newText = `Eu moro em ${ireland.live} e sou apaixonado por ${ireland.love}!`;

    const fruits = 'bannana'
        + `\n`
        + 'orange'
        + `\n`
        + 'apple';

    const newFruits =
        `bannana
orange
apple`;

    console.log(newFruits);

    // console.log(newText);
```

19. 4.2 - Usando Template Literals para Html Fragments

- [Secao-02-Aprendendo-ES6/42-Usando-Template-Literals-para-Htm-Fragments.html](Secao-02-Aprendendo-ES6/42-Usando-Template-Literals-para-Htm-Fragments.html)

```javascript
    const article = {
        title: 'Aprendendo Template Strings',
        intro: 'Uma breve explicação de como se utilizar template strings do ES6 em seu código hoje!',
        body: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestias, officia, perspiciatis? Architecto, molestias autem. Repellat, laborum deserunt soluta necessitatibus. Tenetur illo, id magnam numquam neque illum temporibus, in qui eos.',
        tags: ['es6', 'js', 'template-literal'],
        author: 'José'
    };

    function renderAuthor(name) {
        return (name) ? name : 'unknown';
    }

    const markup = `
    <article>
            <header>
                <h1>${article.title}</h1>
            </header>
            <section>
                <p>${article.intro}</p>
            </section>
            <footer>
                <ul>
                    ${article.tags.map((tag) => `<li>${tag}</li>`).join('')}
                </ul>
                <p>Author: ${renderAuthor(article.author)}</p>
            </footer>
        </article>
    `;

    document.body.innerHTML = markup;
```

20. 4.3 - Tagged Template

- [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)
- [Secao-02-Aprendendo-ES6/43-Tagged-Templat.html](Secao-02-Aprendendo-ES6/43-Tagged-Templat.html)

```javascript
    const city = 'Dubin';
    const something = 'Guinness';
    const otherThing = 'Brasill';

    function green(template, ...values) {
        return template.reduce((acumulador, part, i) => {
            return `
                ${acumulador}
                <span class="green">${values[i -1].toUpperCase()}</span>
                ${part}
            `
        });
    }

    const frase = green`I live in ${city} the city of ${something} and ${otherThing}`;

    document.body.innerHTML = frase;
```

21. 5.1 - Shorthand Properties

- [Secao-02-Aprendendo-ES6/51-Shorthand-Properties.html](Secao-02-Aprendendo-ES6/51-Shorthand-Properties.html)

```javascript
 let firstName = 'José';
    let surname = 'Malcher';
    let age = 36;

    const person = {
        firstName,
        surname,
        age,

        hello(){
            console.log('Hello!!!')
        }
    };

    console.log(person);
    person.hello();
```

22. 5.2 - Default Parameters

- [https://nipher.io/es6-default-parameters/](https://nipher.io/es6-default-parameters/)
- [Secao-02-Aprendendo-ES6/52-Default-Parameters.html](Secao-02-Aprendendo-ES6/52-Default-Parameters.html)

```javascript
   function hello(name = 'José', surname = 'Malcher Jr') {
        console.log(`Hello ${name} ${surname}! How are you?`);
    }

    hello();                  // Hello José Malcher Jr! How are you?
    hello('Jonas', 'Mendes'); // Hello Jonas Mendes! How are you?
    hello('Jonas');           // Hello Jonas Malcher Jr! How are you?
```

23. 5.3 - Novos métodos para Strings

- [Secao-02-Aprendendo-ES6/53-Novos-metodos-para-Strings.html](Secao-02-Aprendendo-ES6/53-Novos-metodos-para-Strings.html)

```javascript
    let text = 'Lorem ipsum dolor sit amet';

    console.log(text.startsWith('rem', 2)); // true
    console.log(text.endsWith('ame', 25));  // true
    console.log(text.includes('ipsum'));   //  true
    console.log('lol'.repeat(10)); // lollollollollollollollollollol
```

24. 6.1 - Array.from()

- [https://exploringjs.com/es6/ch_arrays.html](https://exploringjs.com/es6/ch_arrays.html)
- [Secao-02-Aprendendo-ES6/61-Array-from.html](Secao-02-Aprendendo-ES6/61-Array-from.html)

```html
<ul id="list">
    <li>Jose</li>
    <li>Malcher</li>
    <li>Jr</li>
</ul>

<script>
    const text = 'jose';
    console.log(Array.from(text)); // (4)["j", "o", "s", "e"]

    const list = document.querySelectorAll('#list li'); // (3)[li, li, li]
    const listArray = Array.from(list);
    console.log(listArray);

    const nomes = listArray.map(name => name.textContent);
    console.log(nomes) // (3)["Jose", "Malcher", "Jr"]

</script>
```

25. 6.2 - Array.of()

- [Secao-02-Aprendendo-ES6/62-Array-of.html](Secao-02-Aprendendo-ES6/62-Array-of.html)

```javascript
const array = Array.of(1,4, 'Willian', {name: 'Jonas'});

console.log(array); // (4) [1, 4, "Willian", {…}]

```

26. 6.3 - Array.find() e Array.findIndex()

- [Secao-02-Aprendendo-ES6/63-Array-find-e-Array-findIndex.html](Secao-02-Aprendendo-ES6/63-Array-find-e-Array-findIndex.html)

```javascript
    const data = [
        {
            name: 'Willian',
            age: 26,
            city: 'Dublin'
        },
        {
            name: 'Jonas',
            age: 22,
            city: 'Cologne'
        }
    ];

    const sampleArray = [4, -5, 0, -1];
    const underZero = sampleArray.find(x => x < 0);
    const underZeroIndex = sampleArray.findIndex(x => x < 0);
    //console.log(underZero);      // -5
    //console.log(underZeroIndex); // 1

    const jonas = data.find(person => person.name === 'Jonas');
    const jonasIndex = data.findIndex(person => person.name === 'Jonas');
    console.log(jonasIndex); // 1
```

27. 6.4 - array.fill()

- [Secao-02-Aprendendo-ES6/64-array-fill.html](Secao-02-Aprendendo-ES6/64-array-fill.html)

```javascript
    const arr = new Array(50);
    arr.fill('lol', 3, 6);
    console.log(arr);
    // (50)[empty × 3, "lol", "lol", "lol", empty × 44]

    const newArr = [1,2,3,4,5,6];
    newArr.fill('lol', 1, 3);
    console.log(newArr);
    // (6)[1, "lol", "lol", 4, 5, 6]
```

28. 7.1 - Introdução ao Destructuring

- [https://ponyfoo.com/articles/es6-destructuring-in-depth](https://ponyfoo.com/articles/es6-destructuring-in-depth)

- [Secao-02-Aprendendo-ES6/71-Introducao-ao-Destructuring.html](Secao-02-Aprendendo-ES6/71-Introducao-ao-Destructuring.html)

```javascript
<script>
    var data = {
        name: 'José',
        surname: 'Malcher Jr',
        age: 36,
        blog: 'https://josemalcher.net',
        social: {
            twitter: '@josemalcher',
            facebook: 'fb/josemalcher'
        }
    };

    // const name = data.name;
    // const surname = data.surname;
    // const twitter = data.social.twitter;
    // console.log(name);
    // console.log(surname);
    // console.log(twitter);

    const {name, surname} = data;
    console.log(name);
    console.log(surname);

    const {facebook, twitter} = data.social;
    console.log(facebook)
    console.log(twitter);

    const {facebook: fb} = data.social;
    console.log(fb);

    const {city = 'Belém'} = data; // valor default
    console.log(city);
</script>
```

29. 7.2 - Destructuring em Arrays

- [Secao-02-Aprendendo-ES6/72-Destructuring-em-Arrays.html](Secao-02-Aprendendo-ES6/72-Destructuring-em-Arrays.html)

```javascript
<script>
    const arr = ['Jose', 'Malcher', 36, 'Castanhal-PA'];
    const [name, surname, age, city] = arr;

    console.log(name);
    console.log(surname);
    console.log(age);
    console.log(city);
</script>
```

30. 7.3 - Fazendo swap de variáveis com destructuring

- [Secao-02-Aprendendo-ES6/73-Fazendo-swap-de-variaveis-com-destructuring.html](Secao-02-Aprendendo-ES6/73-Fazendo-swap-de-variaveis-com-destructuring.html)

```javascript
<script>
    let a = 100;
    let b = 999;
    console.log('a = ', a);
    console.log('b = ', b);
    // a =  100
    // b =  999

    [a, b] = [b, a]
    console.log('a = ', a);
    console.log('b = ', b);
    // a =  999
    // b =  100
</script>
```

31. 8.1 - Introdução ao Spread Operator

- [https://ponyfoo.com/articles/es6-spread-and-butter-in-depth](https://ponyfoo.com/articles/es6-spread-and-butter-in-depth)

- [Secao-02-Aprendendo-ES6/81-Introducao-ao-Spread-Operator.html](Secao-02-Aprendendo-ES6/81-Introducao-ao-Spread-Operator.html)

```javascript
<script>
    let front = ['react', 'vue', 'angular'];
    let back = ['python', 'php', 'nodeJS'];

    let fullstack = [...front, 'RxJS', ...back];
    console.log(fullstack);
    // (7)["react", "vue", "angular", "RxJS", "python", "php", "nodeJS"]

    console.log([...'Malcher']); // (7)["M", "a", "l", "c", "h", "e", "r"]
    console.log(...front); // react vue angular

</script>
```

32. 8.2 - Usando o spread dentro de funções

- [Secao-02-Aprendendo-ES6/82-Usando-o-spread-dentro-de-funcoes.html](Secao-02-Aprendendo-ES6/82-Usando-o-spread-dentro-de-funcoes.html)

```javascript
<script>
    function makeSandwich(bread, cheese, sauce) {
        console.log(`Your sandwich with ${bread} bread, ${cheese} cheese and ${sauce} is done!`);
    }

    const ingredients = ['white', 'cheedar', 'berbecue'];
    makeSandwich(...ingredients);
    
    //Your sandwich with white bread, cheedar cheese and berbecue is done!

</script>
```

33. 8.3 - Rest params

- [Secao-02-Aprendendo-ES6/83-Rest-params.html](Secao-02-Aprendendo-ES6/83-Rest-params.html)

```javascript
<script>
    function multiply(mult, ...args) {
        return args.map(arg => arg * mult);
    }

    console.log(multiply(10, 1, 2, 3, 4, 5));
    // (5)[10, 20, 30, 40, 50]

</script>
```

34. 9.1 - Introdução a Promises

- [https://ponyfoo.com/articles/es6-promises-in-depth](https://ponyfoo.com/articles/es6-promises-in-depth)
- [https://nipher.io/es6-promises/](https://nipher.io/es6-promises/)

- [Secao-02-Aprendendo-ES6/91-Introducao-a-Promises.html](Secao-02-Aprendendo-ES6/91-Introducao-a-Promises.html)

```javascript
<script>
    var defer = new Promise((resolve, reject) => {
        setTimeout(() => {
            if (true) {
                resolve('Hello! It Work');
            } else {
                reject('Error');
            }
        }, 2000);
    });

    defer
        .then((data) => {
            console.log(data);
            return 'fooooo';
        })
        .then((data) => console.log(data))
        .catch((err) => console.log(err));
    // Hello! It Work
    // fooooo
</script>
```

35. 9.2 - Exemplo Real de Promises

- [https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

- [Secao-02-Aprendendo-ES6/92-Exemplo-Real-de-Promises.html](Secao-02-Aprendendo-ES6/92-Exemplo-Real-de-Promises.html)

```javascript
<script>
    var post = fetch('https://josemalcher.net/wp-json/wp/v2/posts');

    // pending
    // resolved
    // rejected

    post
        .then(data => data.json())
        .then(data => data.map(post=>{
            console.log(post.title);
        }));
</script>
```

36. 9.3 - Manipulando múltiplas Promises

- [Secao-02-Aprendendo-ES6/93-Manipulando-multiplas-Promises.html](Secao-02-Aprendendo-ES6/93-Manipulando-multiplas-Promises.html)

```javascript
<script>
    const currency = new Promise((resolve, reject) => {
        setTimeout(() => {
            resolve({currency: 'euro', value: 3.50});
        }, 5000);
    });

    const countries = new Promise((resolve, reject) => {
        resolve(['Ireland', 'England', 'Scotland']);
    });

    // Promise
    //     .all([currency, countries]) // as duas são resolvidas
    //     .then(responses => {
    //         console.log(responses);
    //     })

    Promise
        .race([currency, countries]) // quem responde primeiro é resolvida
        .then(responses => {
            console.log(responses);
        })
</script>
```

37. 10.1 - Herança Prototipal

- [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)

- [Secao-02-Aprendendo-ES6/101-HerancaPrototipal.html](Secao-02-Aprendendo-ES6/101-HerancaPrototipal.html)

```javascript
<script>
  //class
  function Animal(kind, sound) {
    //constructor
    this.kind = kind;
    this.sound = sound;
  }

  //methods
  Animal.prototype.hello = function () {
    console.log(`${this.sound} I'm a ${this.kind}`);
  };

  const dog = new Animal('dog', 'AUAUAUAU');
  const cat = new Animal('Cat', 'meouww');

</script>
```

38. 10.2 - Criando Classes do ES6

39. 10.3 - Usando extended classes

40. 11.1 - Introdução a Symbols

41. 11.2 - Iterators e Iterables - for...of

42. 12.1 - Introdução a Generators

43. 12.2 - Usando Generators para fluxos assíncronos

44. 13.1 - Introdução ao Proxy

45. 14.1 - Introdução ao Set

46. 14.2 - Introdução ao WeakSet

47. 15.1 - Introdução ao Map

48. 15.2 - Introdução ao WeakMap


[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Seção 3: Atualizações ES7/ES8</a>



[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Seção 4: Módulos em JS</a>



[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Seção 5: Teoria de Testes</a>



[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Seção 6: Unindo conceitos na prática</a>



[Voltar ao Índice](#indice)

---


## <a name="parte7">7 - Seção 7: Criando uma Biblioteca Wrapper da API do Spotify</a>



[Voltar ao Índice](#indice)

---


## <a name="parte8">8 - Seção 8: Refatorando uma biblioteca com testes</a>



[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Seção 9: Criando um Player do Spotify</a>



[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Seção 10: Criando uma CLI para converter Bitcoin em qualquer moeda</a>



[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Seção 11: Introdução a Testes com React - Criando um Componente Full Header</a>



[Voltar ao Índice](#indice)

---


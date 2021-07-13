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

20. 4.3 - Tagged Template

21. 5.1 - Shorthand Properties

22. 5.2 - Default Parameters

23. 5.3 - Novos métodos para Strings

24. 6.1 - Array.from()

25. 6.2 - Array.of()

26. 6.3 - Array.find() e Array.findIndex()

27. 6.4 - array.fill()

28. 7.1 - Introdução ao Destructuring

29. 7.2 - Destructuring em Arrays

30. 7.3 - Fazendo swap de variáveis com destructuring

31. 8.1 - Introdução ao Spread Operator

32. 8.2 - Usando o spread dentro de funções

33. 8.3 - Rest params

34. 9.1 - Introdução a Promises

35. 9.2 - Exemplo Real de Promises

36. 9.3 - Manipulando múltiplas Promises

37. 10.1 - Herança Prototipal

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


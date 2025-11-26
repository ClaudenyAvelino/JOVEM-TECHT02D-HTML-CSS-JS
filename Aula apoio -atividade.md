# 📘 Conteúdo Detalhado – Dia 1 (JavaScript Básico)

## 🟡 1. O que é JavaScript? Onde é usado (Front-End)?

**JavaScript (JS)** é uma linguagem de programação voltada principalmente para o **desenvolvimento web**. Ele é responsável por dar **interatividade às páginas**, funcionando junto com:

- **HTML** (estrutura)
- **CSS** (estilo)

### Exemplos de uso no Front-End:
- Criar menus interativos
- Validar formulários
- Mostrar ou esconder elementos na tela
- Fazer animações simples
- Atualizar conteúdo sem recarregar a página

### 💡 Demonstração:
Use uma página estática (HTML + CSS) e outra com um botão que muda a cor de fundo ou exibe um alerta. Explique que o JS é o responsável por essa "magia".

---

## 🟡 2. Inserção do JS no HTML (`<script>`)

### Formas de usar JavaScript em uma página:

#### 🔸 JS Interno:
```html
<script>
  alert("Olá, mundo!");
</script>
```
🔸 JS Externo (melhor prática):
```
<!-- HTML -->
<script src="script.js"></script>
```

✅ Boa prática:

```
<script> antes do </body>
```

> Coloque a tag para garantir que o HTML seja carregado primeiro, evitando erros ao acessar elementos da página.



🟡 3. Console e console.log()
O que é o Console?

Ferramenta dos navegadores para visualizar mensagens de depuração.

Acesse com F12 > Aba "Console" (Chrome, Firefox, Edge).

Uso básico:
```
console.log("Bem-vindo ao JavaScript!");

```
💡 Demonstração:

Alunos para abrirem o console do navegador e usarem console.log() para exibir mensagens e variáveis.

🟡 4. Variáveis e Tipos Primitivos
O que são variáveis?

Espaços de memória para armazenar informações.

🧾 Declarações em JS:

```
var nome = "João";      // forma antiga (evitar)
let idade = 25;         // recomendado
const pi = 3.14;        // constante (não muda)
```

🧠 Tipos primitivos:

```
| Tipo      | Exemplo              |
| --------- | -------------------- |
| String    | `"texto"`            |
| Number    | `10`, `3.14`         |
| Boolean   | `true`, `false`      |
| Undefined | `let x;` (sem valor) |
| Null      | `let x = null;`      |
```

👨‍💻 Demonstração:
```
let nome = "Maria";       // string
let idade = 30;           // number
let estudante = true;     // boolean

console.log(nome);
console.log(typeof idade);       // number
console.log(typeof estudante);   // boolean
console.log(typeof nome);        // string
console.log(typeof idade);       // number
console.log(typeof estudante);   // boolean
```

🟡 5. Operadores Matemáticos e Lógicos
➤ Matemáticos:

```
let a = 10;
let b = 5;

console.log(a + b);  // 15
console.log(a - b);  // 5
console.log(a * b);  // 50
console.log(a / b);  // 2
console.log(a % b);  // 0 (resto da divisão)
```
➤ Atribuição com operadores:

```
a += 2; // equivalente a: a = a + 2

```

➤ Comparação:

```
a == b     // igualdade (valor)
a === b    // igualdade (valor e tipo)
a != b     // diferente
a > b
a < b
```

➤ Lógicos:

```
true && false   // false (E)
true || false   // true  (OU)
!true           // false (NÃO)
```

💡 Exemplo prático:

```
let idade = 18;
let temCarteira = true;

if (idade >= 18 && temCarteira) {
  console.log("Pode dirigir!");
} else {
  console.log("Não pode dirigir.");
}
```

🟡 6. Comentários

Comentário de uma linha:

```
// Isso é um comentário
```

Comentário de múltiplas linhas:

```
/*
  Este é um comentário
  de várias linhas
*/
```
---
💡 Dica:

Os alunos a usarem comentários para explicar partes do código.

---

🧪 7. Atividade prática

Crie um arquivo HTML com um script JS externo. No JS, os alunos devem:

Declarar variáveis dos tipos: string, number e boolean

Exibir essas variáveis no console usando console.log

Fazer uma conta simples (ex: soma de dois números)

Usar uma estrutura condicional if para verificar uma condição e exibir uma mensagem
----
📁 8. Estrutura de pastas sugerida:

```
aula01-js/
│
├── index.html
└── script.js
```


📁 08/10/2025
<a href="https://1drv.ms/b/c/08a6d1d355a14254/EekiPdG7DF5HoyC8tHmB1KIB68XEELu7CvE7NEuPAYGsPQ?e=sz4afg">Atividade</a>

---
🟡 9. Estruturas de Controle (Laços de Repetição)

Essencial para lógica de programação.

➤ for, while, do...while

```
for (let i = 0; i < 5; i++) {
  console.log("Número: " + i);
}

let j = 0;
while (j < 5) {
  console.log("Contando: " + j);
  j++;
}
```

---
💡 Atividade prática: Mostrar os números pares de 0 a 10 com for.

---
🟡 10. Funções
➤ Declaração e chamada de funções

```
function saudacao(nome) {
  console.log("Olá, " + nome + "!");
}

saudacao("Ana");
```

---
➤ Funções com retorno:

```
function soma(a, b) {
  return a + b;
}

let resultado = soma(2, 3);
console.log(resultado);
```
---
💡 Atividade: Criar uma função que calcula o IMC.
---

🟡 11. Arrays (Vetores)

```
let frutas = ["maçã", "banana", "laranja"];

console.log(frutas[0]);       // maçã
console.log(frutas.length);   // 3

frutas.push("uva");           // adiciona
frutas.pop();                 // remove o último
```

---

💡 Atividade: Criar um array com nomes e exibir todos com um for.
---

🟡 12. Objetos.

```
let pessoa = {
  nome: "João",
  idade: 30,
  profissao: "Dev"
};

console.log(pessoa.nome);
```
---

💡 Atividade: Criar um objeto "carro" com marca, modelo e ano.

---

🟡 13. Manipulação do DOM (mais detalhado)

➤ getElementById, querySelector, innerText, innerHTML, style
```
document.getElementById("meuBotao").addEventListener("click", function() {
  document.body.style.backgroundColor = "blue";
});
```

💡 Demonstração prática: Criar uma página com botão que muda texto, cor, ou esconde um bloco.

---

🟡 14. Eventos

➤ click, mouseover, keydown, etc.

```
document.getElementById("meuBotao").onclick = function() {
  alert("Botão clicado!");
};
```
---
# 📚 Aula: Manipulação do DOM com JavaScript

## 🟡 Slide 1 – Título
**Manipulação do DOM com JavaScript**

**Conteúdos abordados:**
- `getElementById`, `querySelector`
- `innerText`, `innerHTML`
- `style`
- Eventos com `addEventListener`

---

## 🟡 Slide 2 – O que é DOM?

- **DOM** = *Document Object Model*
- Representa a página HTML como uma **árvore de objetos**
- JavaScript pode **acessar e modificar** elementos HTML

📌 **Exemplo:**

```html
<div id="exemplo">Olá</div>
```
![DOM HTML](/img/dom.jpg "Manipulando DOM com JavaScript")


---
```
document.getElementById("exemplo").innerText = "Novo texto!";
```

🟡 Slide 3 – Seletores DOM

🔹 Métodos mais usados:

```document.getElementById("id")
document.querySelector("seletor CSS")
document.querySelectorAll("seletor CSS")
```

📌 Exemplos:

```document.getElementById("titulo")
document.querySelector(".minhaClasse")
document.querySelector("#meuBotao")
```

👨‍🏫 Demonstração – Passo a passo:

HTML de exemplo:
```<h1 id="titulo">Bem-vindo</h1>
<p class="texto">Parágrafo 1</p>
<p class="texto">Parágrafo 2</p>
<div id="caixa">
  <p>Conteúdo da caixa</p>
</div>
```
Abrir DevTools (F12) e usar o Console:

```
// 👉 getElementById
document.getElementById("titulo")

// 👉 querySelector
document.querySelector(".texto")

// 👉 querySelectorAll
document.querySelectorAll(".texto")
```

📝 Observações:

querySelector retorna o primeiro elemento que combina.

querySelectorAll retorna todos os elementos.

💡 Modificando visualmente:

```
document.getElementById("titulo").innerText = "Novo Título!";
document.querySelector("#caixa").style.backgroundColor = "lightgreen";
```

🟡 Slide 4 – Modificando Conteúdo

```
element.innerText = "Texto comum";
element.innerHTML = "<strong>Texto em negrito</strong>";
```

✅ innerText: exibe apenas texto
✅ innerHTML: interpreta HTML

🟡 Slide 5 – Estilizando com JS

```
element.style.color = "blue";
element.style.backgroundColor = "yellow";
element.style.display = "none";
```

📌 É possível alterar qualquer estilo CSS via JavaScript!


🟡 Slide 6 – Eventos com addEventListener

```
element.addEventListener("click", function() {
  // ação a ser executada
});
```

🎯 Eventos comuns:

click
input
mouseover
submit

---
🟡 Slide 7 – Demonstração prática

🎯 Exercício:

Criar uma página com:

Um bloco de texto

Três botões:

Mudar o texto

Mudar a cor de fundo

Esconder ou mostrar o bloco

```
<div id="meuBloco">
  <p id="textoBloco">Este é o texto original.</p>
</div>

<button id="btnTexto">Alterar Texto</button>
<button id="btnCor">Mudar Cor</button>
<button id="btnEsconder">Esconder/Mostrar</button>
```

🟡 Slide 9 – Código JavaScript externo

```
const bloco = document.getElementById("meuBloco");
const texto = document.querySelector("#textoBloco");

document.getElementById("btnTexto").addEventListener("click", function() {
  texto.innerText = "O texto foi alterado com sucesso!";
});

document.getElementById("btnCor").addEventListener("click", function() {
  bloco.style.backgroundColor = "lightblue";
});

document.getElementById("btnEsconder").addEventListener("click", function() {
  bloco.style.display = bloco.style.display === "none" ? "block" : "none";
});
```

🟡 Slide 10 – Lição de casa

🎯 Crie uma página com:

Um título

Um campo de input

Um botão “Enviar”

Ao clicar, exibir a mensagem:

📢 "Olá, [nome digitado]!"

💡 Dica: Use getElementById, innerText, style, e click

---


💡 Atividade: Criar uma caixa de texto e exibir o que foi digitado em tempo real (evento input).
---

🟡 15 Conversão de Tipos

```
let numero = "10";
console.log(Number(numero)); // 10 (number)

```

💡 Atividade: Soma de dois números digitados pelo usuário (inputs) e mostrar o resultado.




---
# 🧭 Atividade Prática – Projeto “Meu Primeiro Site Comercial”

>⚠️ Aviso: **Não é permitido:** Utilizar ferramentas de Inteligência Artificial (IA), como ChatGPT, Bing Chat, Gemini, etc.

> ✅ **Você pode utilizar:**
 <ol>
  <li>Seu caderno ou anotações pessoais.</li>
  <li>O manual de HTML, CSS e JavaScript apresentado pelo professor.
      <ol>
      <li>https://www.w3schools.com/</li>
      <li>https://htmldog.com/references/html/</li>
      <li>https://html.com/html5/</li>
      <li>https://color.adobe.com/pt/create/color-wheel</li>
      <li>https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/script</li>
    </ol>
  </li>
  <li>Materiais didáticos utilizados durante as aulas
    <ol>
      <li>https://github.com/ClaudenyAvelino/JOVEM-TECHT02D-LOGICA</li>
      <li>https://github.com/ClaudenyAvelino/html-basico</li>
       <li>https://github.com/ClaudenyAvelino/JOVEM-TECHT02D-HTML-CSS-JS</li>
    </ol>
  </li>
</ol>



## 🎯 Objetivo da atividade:
Aplicar na prática os conhecimentos de HTML, CSS e JavaScript, desenvolvendo um site completo e funcional para um comércio local.

---

## 🧱 Descrição da atividade:
Cada grupo deverá **sair a campo individualmente** e **prospectar um cliente real** em comércio local. — podendo ser:

- Um **comércio local** (mercadinho, lanchonete, loja de roupas, salão de beleza, etc.);  
- Ou um **empreendimento de artesanato** (loja, feirante, artista local, oficina artesanal, etc.).  

O grupo deverá conversar com o responsável pelo negócio para compreender:  
- O que o comércio oferece (produtos ou serviços);  
- As informações que o cliente gostaria de divulgar no site (nome, endereço, contato, redes sociais, etc.);  
- E o **estilo visual desejado** (cores, imagens, logotipo, etc.).

---

## 💻 Entrega:
Desenvolver um **site simples e funcional** com:

1. **HTML:** estrutura básica e seções organizadas (`header`, `main`, `section`, `footer`)  
2. **CSS:** estilização personalizada, cores e layout atrativo  
3. **JavaScript:** pelo menos uma **interatividade funcional**, como:
   - Botão de alterar cor de fundo  
   - Alerta de boas-vindas  
   - Validação simples de formulário  
   - Exibição de mensagem automática  

---

## 📌 Boas práticas:
- Use **HTML semântico** para melhorar a acessibilidade e SEO.  
- Mantenha **CSS organizado** e reutilizável, evitando estilos inline quando possível.  
- Use **JavaScript externo** (`script.js`) e carregue-o antes do fechamento do `</body>`.  
- Nomeie **classes e IDs** de forma clara e consistente.  
- Teste o site em diferentes navegadores e tamanhos de tela (responsividade).  
- Inclua **comentários** explicativos no código para facilitar a manutenção.  
- Evite usar cores e fontes que prejudiquem a leitura.  

---

## 🧠 Critérios de avaliação:

| Critério                     | Descrição                                           | Pontos |
|-------------------------------|---------------------------------------------------|--------|
| Estrutura HTML                | Uso correto das tags semânticas e organização do conteúdo | 2,0    |
| Estilo CSS                    | Aplicação de layout, cores e design coerente com o tema | 2,0    |
| Interatividade JS             | Funcionalidade implementada corretamente         | 2,0    |
| Criatividade e identidade visual | Originalidade e adequação ao negócio escolhido | 2,0    |
| Entrevista e compreensão do cliente | Clareza nas informações obtidas do comércio/artesanato | 2,0    |
| **Total**                     |                                                   | **10,0** |
---

📂 Organização do projeto (estrutura de pastas):

```meu-site-comercial/
│
├── index.html
├── style.css
└── script.js
```

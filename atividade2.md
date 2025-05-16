## Atividade 2: Analisando a Validação de Formulários com JavaScript

A **validação de formulários** é usada para garantir que os dados digitados pelos usuários estão corretos antes de serem enviados para o servidor. 
Com JavaScript, essa validação é feita **no lado do cliente**, ou seja, no próprio navegador, o que evita o envio de dados inválidos e melhora a experiência do usuário.

## Como o JavaScript faz a validação?

**1-Captura os dados do formulário**: usando o DOM(representação estruturada de um documento HTML (ou XML) em forma de árvore, que o navegador usa para representar e interagir com os elementos da página), o JavaScript acessa os campos preenchidos.

```javascript
 let nome = document.getElementById("nome").value;
```
**2-Verifica se os dados são válidos:** por exemplo, se o campo está vazio ou se segue um padrão.

```javascript
if (nome === "") {
  alert("Por favor, preencha o nome.");
}
```
**3-Impede o envio se houver erro:** normalmente usando *event.preventDefault().*

```javascript
document.getElementById("formulario").addEventListener("submit", function(event) {
  if (nome === "") {
    alert("Nome obrigatório");
    event.preventDefault(); // impede o envio
  }
});
```
# Regex
As expressões regulares (regex) são padrões usados para verificar se um dado tem a estrutura correta. Um exemplo comum é validar e-mails.
*Regex para email*: expressão regular que define um padrão para validar ou identificar endereços de email.

**Exemplo de regex para e-mail:**

```javascript
let email = document.getElementById("email").value;
let padrao = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

if (!padrao.test(email)) {
  alert("E-mail inválido");
}
```
**Explicação do padrão:**

*^[^\s@]+* → Começa com um ou mais caracteres que não são espaço nem @

*@* → Deve conter o símbolo "@"

*[^\s@]+* → Depois do @, mais caracteres válidos

*\.* → Um ponto (.)

*[^\s@]+$* → Termina com uma parte válida depois do ponto (como ".com", ".br", etc.)


## Fontes:

https://developer.mozilla.org/pt-BR/docs/Learn/Forms/Form_validation

https://www.w3schools.com/js/js_validation.asp

https://javascript.info/form-elements

https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Regular_Expressions

https://regex101.com/

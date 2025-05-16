# Atividade 3 – Detalhando a Arquitetura Cliente-Servidor na Web

## O que é a arquitetura cliente-servidor?

A **arquitetura cliente-servidor** é um modelo onde dois lados se comunicam:
- **Cliente**: geralmente o navegador (Chrome, Firefox, etc.)
- **Servidor**: computador remoto onde está hospedado o site

## Passo a passo de como um site carrega

1. **O usuário digita o endereço do site** (como www.exemplificacao.com) no navegador.

2. **Consulta ao DNS (Domain Name System)**: o navegador pergunta para o DNS qual é o endereço IP do site (por exemplo, "142.250.72.14"). O DNS funciona como uma agenda telefônica da internet.

3. **Requisição HTTP**: o navegador envia uma **requisição HTTP** para o servidor, pedindo a página:

*Host:* www.exemplificacao.com

**4-Resposta HTTP**: o servidor responde com a página pedida, usando o protocolo HTTP:

HTTP/1.1 200 OK
Content-Type: text/html

```javascript
<html>...</html> 
```
**5-Renderização da página:** o navegador pega o HTML e começa a exibir o conteúdo na tela. Se a página tiver CSS, JavaScript, imagens, etc., ele faz novas requisições para carregar tudo.

**6-Interação do usuário:** o usuário clica, digita ou interage, e o navegador pode enviar novas requisições para o servidor, se necessário (como para enviar um formulário).

## Fontes:
https://developer.mozilla.org/pt-BR/docs/Learn/Getting_started_with_the_web/How_the_Web_works

https://www.w3schools.com/whatis/whatis_http.asp

https://www.cloudflare.com/pt-br/learning/dns/what-is-dns/

https://www.geeksforgeeks.org/client-server-architecture/

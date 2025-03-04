# 📄 Documentação do Código HTML

Este código HTML cria uma página web simples com um formulário de busca que redireciona o usuário para os resultados do Google. Abaixo está a explicação detalhada de cada parte do código.

---

## 🎥 Demonstração em Vídeo

Confira abaixo um vídeo demonstrativo do funcionamento do formulário:

https://github.com/user-attachments/assets/716d9f03-69c4-4fb1-ac60-f5777c475b3c

---

## 🛠️ Estrutura do Código

### 1. **Declaração do Tipo de Documento (`<!DOCTYPE html>`)**
   - Indica que o documento está escrito em **HTML5**.

### 2. **Elemento `<html>`**
   - Define o início do documento HTML.
   - O atributo `lang="pt-br"` especifica que o conteúdo da página está em **português do Brasil**.

### 3. **Elemento `<head>`**
   - Contém metadados sobre o documento, como o conjunto de caracteres e o título da página.

   - **Elemento `<meta charset="UTF-8">`**
     - Define o conjunto de caracteres como **UTF-8**, garantindo a correta exibição de caracteres especiais.

   - **Elemento `<title>`**
     - Define o título da página, que aparece na aba do navegador. Neste caso, o título é **"Formulário de busca"**.

### 4. **Elemento `<body>`**
   - Contém o conteúdo visível da página.

   - **Elemento `<h1>`**
     - Exibe um cabeçalho de nível 1 com o texto **"Formulário de busca"**.

   - **Elemento `<form>`**
     - Define um formulário que envia os dados para o Google.
     - **Atributos:**
       - `action="https://www.google.com.br/search"`: Especifica a URL para onde os dados do formulário serão enviados.
       - `method="get"`: Define o método HTTP como **GET**, o que significa que os dados do formulário serão anexados à URL.
       - `target="_blank"`: Abre os resultados da busca em uma **nova aba/janela**.

     - **Elemento `<label>`**
       - Associa um rótulo ao campo de entrada de texto. O atributo `for="busca"` vincula o rótulo ao campo com o ID correspondente.

     - **Elemento `<input type="text">`**
       - Cria um campo de texto onde o usuário pode digitar o termo de busca.
       - **Atributos:**
         - `name="q"`: Define o nome do campo, que será usado para enviar o termo de busca ao Google.
         - `id="busca"`: Identifica o campo para ser associado ao rótulo.

     - **Elemento `<input type="submit">`**
       - Cria um botão de envio com o texto **"OK"**. Quando clicado, o formulário é enviado.

---

## 🚀 Como Funciona
1. O usuário digita um termo de busca no campo de texto.
2. Ao clicar em **"OK"**, o formulário envia o termo de busca para o Google.
3. Os resultados da busca são exibidos em uma **nova aba/janela** do navegador.

---

## 💻 Exemplo de Uso

Aqui está o código completo para referência:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Formulário de busca</title>
</head>
<body>
    <h1>Formulário de busca</h1>
    <form action="https://www.google.com.br/search" method="get" target="_blank">
        <label for="busca">Faça uma busca: </label>
        <input type="text" name="q" id="busca">
        <input type="submit" value="OK">
    </form>
</body>
</html>

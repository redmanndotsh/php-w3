# php-w3
Repo for W3Schools PHP tutorials files and exercises (🇧🇷 PT-BR)

## Visão geral
- PHP: linguagem de lado servidor
- Ferramenta poderosa para a criação de páginas web dinâmicas e interativas
- Largamente usado
- Software livre
- Alternativa eficiente às concorrentes, como ASP (da Microsoft)
- Até o presente momento (15/01/2019), o PHP 7 é a última versão estável

## Introdução
- Linguagem de lado servidor (ou Server Side Language): o código é executado no servidor

### O que você já deve saber
Antes de começar a estudar PHP, é recomendável que você já saiba o básico dos seguintes tópicos
- HTML
- CSS
- JavaScript

### O que é
- *PHP*: acrônimo recursivo para **PHP: Hypertext Preprocessor**
- Largamente usado
- Linguagem de script open-source
- Scripts PHP são executados no servidor da aplicação, não no navegador do cliente
- Gratuito para baixar e livre para usar
- Poder: está no núcleo do WordPress e roda o Facebook
- Facilidade: pode ser a primeira linguagem de lado servidor para um iniciante

### Arquivo PHP
- Um arquivo PHP pode conter: Texto, HTML, CSS, JavaScript e **Código PHP**
- Fluxo: códigos PHP executados no servidor e resultados exibidos no navegador
- Extensão: **.php**

### O que pode fazer
- Gerar conteúdo dinâmico para páginas web
- Arquivos no servidor: criação, leitura, escrita e deleção
- Coletar dados de formulários HTML
- Enviar e receber cookies
- Banco de dados: adição, deleção e modificação de dados
- Controlar acesso de usuários
- Encriptar dados

> Não limitado a HTML: imagens, PDFs, conteúdo flash, texto, XHTML e XML

### Por que usar
- Multiplataforma: Windows, Linux, Mac OS, etc
- Compatibilidade com a maioria dos servidores web usados atualmente
- Suporte a um largo número de bancos de dados
- PHP é grátis e livre: http://www.php.net/
- PHP é fácil de aprender e roda eficientemente no servidor

### Ambiente PHP
Para os arquivos PHP serem lidos corretamente, você precisa configurar um servidor web. Ele deve suportar PHP. Configurá-lo pode ser trabalhoso, então você pode baixar o [XAMPP](https://www.apachefriends.org/index.html). O XAMPP é uma distibuição Apache que carrega junto consigo o MariaDB, o PHP e o Perl.
> Após a instalação, rode o XAMPP e acesse [localhost](http://localhost).
Caso tudo tenha corrido bem, você deverá ver uma página como esta:
![image](https://user-images.githubusercontent.com/24627793/72675600-765aee00-3a65-11ea-8fca-340f014b2b40.png)

#### Atenção
A instalação gerará uma pasta chamada **htdocs**. É lá onde colocaremos nossos arquivos PHP.

## Síntaxe PHP
Um script PHP se inicia com ```<?php``` e se encerra com ```?>```
- Scripts PHP podem ser colocados em qualquer lugar do documento .php

### Exemplo 01: arquivo PHP simples
```php
<?php
  // o código PHP fica exatamente entre esses dois conjuntos de simbolos
?>
```
**A extensão padrão de arquivos PHP é .php**

- Geralmente, um arquivo PHP contém tags HTML e alguns códigos de script
- O arquivo acima não gera conteúdo algum, veremos mais adiante porquê

### Exemplo 02: imprimindo o "Olá, mundo!"

```php
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8">
  </head>
  <body>
    <h1>Minha primeira página PHP</h1>

    <?php
      echo "Olá, mundo!";
    ?>
  </body>
</html>
```

- O código acima parece pertencer a um arquivo de extensão .html, mas é .php
- Entre a sexta e a oitava linha, podemos observar um código PHP. Na sétima, fazemos uso de uma função bult-in. ```echo``` imprime conteúdo na tela do usuário.
- Comandos PHP terminam com **ponto-e-vírgula**

### PHP é case sensitive?
- Palavras-chave: **não** case sensitive
- Classes: **não** case sensitive
- Funções: **não** case sensitive
- **Variáveis**: case sensitive

#### Exemplo 03: testando o case sensibility

```php
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8">
  </head>
  <body>
    <h1>Minha primeira página PHP</h1>

    <?php
      ECHO "Olá, mundo!";
      echo "Olá, mundo!";
      EcHo "Olá, mundo!";
    ?>
  </body>
</html>
```

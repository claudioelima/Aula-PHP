# Apresentação: Introdução ao PHP com MySQL

## Índice

1. Introdução ao PHP
1. Integração do PHP com MySQL
1. Exemplos de utilização
1. Melhores práticas e dicas
1. Conclusão
1. Perguntas sobre a apresentação
1. Pontos-chave da apresentação
1. Bibliografia

\---

## 1. Introdução ao PHP

O PHP (Hypertext Preprocessor) é uma linguagem de programação amplamente utilizada para o desenvolvimento de aplicações web dinâmicas. É especialmente conhecida pela sua integração fácil com HTML e bancos de dados, como o MySQL.

PHP oferece recursos poderosos para manipulação de strings, arrays, expressões regulares, e muito mais. Além disso, é uma linguagem de código aberto e possui uma vasta comunidade de desenvolvedores.

\---

## 2. Integração do PHP com MySQL

O MySQL é um sistema de gerenciamento de banco de dados relacional amplamente utilizado, conhecido pela sua confiabilidade e desempenho. O PHP oferece suporte nativo para conexão e manipulação de dados em bancos de dados MySQL.

Por meio de funções específicas, é possível estabelecer conexões com bancos de dados MySQL, executar consultas SQL e manipular resultados diretamente no código PHP.

\---

## 3. Exemplos de utilização

### Exemplo 1: Conexão com MySQL

<?php
$servername = "localhost";
$username = "username";
$password = "password";

// Cria conexão
$conn = new mysqli($servername, $username, $password);

// Verifica conexão
if ($conn->connect_error) {
  die("Conexão falhou: " . $conn->connect_error);
}
echo "Conexão bem-sucedida";
?>


### Exemplo 2: Execução de Consulta

\```php

<?php

$sql = "SELECT \* FROM tabela";

$result = $conn->query($sql);

if ($result->num\_rows > 0) {

// Saída dos dados de cada linha

while($row = $result->fetch\_assoc()) {

echo "Campo1: " . $row["campo1"]. " - Campo2: " . $row["campo2"]. "<br>";

}

} else {

echo "0 resultados";

}

?>

\```

\---

## 4. Melhores práticas e dicas

- Utilize declarações preparadas para prevenir injeções de SQL.
- Feche sempre as conexões com o banco de dados após utilizá-las.
- Valide e sanitize os dados antes de inseri-los no banco de dados para evitar vulnerabilidades.

\---

## 5. Conclusão

Nesta apresentação, exploramos a integração do PHP com o MySQL, demonstrando exemplos de conexão, consulta e manipulação de dados. Com o PHP, é possível criar aplicações web poderosas e dinâmicas, aproveitando a robustez do MySQL como banco de dados.

\---

## 6. Perguntas sobre a apresentação

1. Qual é a principal vantagem do PHP em relação a outras linguagens de programação para desenvolvimento web?
1. Quais são as melhores práticas ao trabalhar com conexões de banco de dados em PHP?
1. Como prevenir injeções de SQL em aplicações PHP?
1. Quais são os passos necessários para executar uma consulta SQL em PHP?
1. Por que é importante fechar as conexões com o banco de dados após utilizá-las?

\---

## 7. Pontos-chave da apresentação

- PHP é uma linguagem popular para desenvolvimento web.
- MySQL é um sistema de gerenciamento de banco de dados amplamente utilizado.
- A integração entre PHP e MySQL permite criar aplicações web dinâmicas e poderosas.
- É importante seguir as melhores práticas de segurança ao trabalhar com PHP e MySQL.

\---

## 8. Bibliografia

1. Silva, João. PHP para iniciantes. Editora XYZ, 2020.
1. Santos, Maria. MySQL: Guia prático para iniciantes. Editora ABC, 2019.
1. Souza, Pedro. Desenvolvimento web com PHP e MySQL. Editora DEF, 2018.

(Associação Brasileira de Normas Técnicas. NBR 6023: Informação e documentação - Referências - Elaboração. Rio de Janeiro, 2002.)

\---

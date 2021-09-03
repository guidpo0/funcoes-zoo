### Informações Gerais

Projeto desenvolvido durante formação em desenvolvedor Web Full Stack pela Trybe.

---

# Boas vindas ao repositório do projeto de ES6 e Higher Order Functions!

Este projeto consiste em resolver desafios utilizando as HOF's!

Lembrando que esta aplicação corresponde aos meus esforços para melhorar minhas hard skills e soft skills, sinta-se à vontade para explorá-la! Feedbacks construtivos são sempre bem vindos!

Abaixo você poderá encontrar mais informações técnicas sobre este projeto.

---

## Sumário

- [Habilidades](#habilidades)
- [Intruções para fazer o fork do repositório](#intruções-para-fazer-o-fork-do-repositório)
- [Informações do projeto](#informações-do-projeto)
  - [Linter](#linter)
  - [Estrutura](#estrutura)
- [Desafios](#desafios)
  - [1. Implemente a função getSpeciesByIds](#1-implemente-a-função-getSpeciesByIds)
  - [2. Implemente a função getAnimalsOlderThan](#2-implemente-a-função-getAnimalsOlderThan)
  - [3. Implemente a função getEmployeeByName](#3-implemente-a-função-getEmployeeByName)
  - [4. Implemente a função createEmployee](#4-implemente-a-função-createEmployee)
  - [5. Implemente a função isManager](#5-implemente-a-função-isManager)
  - [6. Implemente a função addEmployee](#6-implemente-a-função-addEmployee)
  - [7. Implemente a função countAnimals](#7-implemente-a-função-countAnimals)
  - [8. Implemente a função calculateEntry](#8-implemente-a-função-calculateEntry)
  - [9. Implemente a função getAnimalMap](#9-implemente-a-função-getAnimalMap)
  - [10. Implemente a função getSchedule](#10-implemente-a-função-getSchedule)
  - [11. Implemente a função getOldestFromFirstSpecies](#11-implemente-a-função-getOldestFromFirstSpecies)
  - [12. Implemente a função increasePrices](#12-implemente-a-função-increasePrices)
  - [13. Implemente a função getEmployeeCoverage](#13-implemente-a-função-getEmployeeCoverage)

---

## Habilidades

Nesse projeto, fui capaz de:

- Produzir código legível, conciso e expressivo utilizando as novas funcionalidades do ES6
- Utilizar as _Higher Order Functions_ para manipular e criar arrays
- Escolher a _Higher Order Function_ mais adequada para a obtenção de um resultado esperado
- Aprender a usar de forma conjunta as _Higher Order Functions_
- Interpretar testes unitários e produzir soluções que atendam a eles

---

# Instruções para fazer o fork do repositório

1. Faça o fork do repositório

2. Instale as dependências do projeto
  * Instale as dependências:
    * `npm install`

---

# Informações do projeto

### Linter

Para garantir a qualidade do código de forma a tê-lo mais legível, de mais fácil manutenção e seguindo as boas práticas de desenvolvimento foi utilizado neste projeto o linter `ESLint`.

### Estrutura

Na pasta raiz do projeto, temos a pasta `src` e a pasta `tests`. A pasta `src` é composta pelo arquivo `zoo.js`, que contém as funções implementadas, e o arquivo `data.js`, que armazena os dados que serão utilizados. Já a pasta `tests`, contém os testes unitários correspondentes a cada função do arquivo `zoo.js`.

O nome dos arquivos também segue uma ordem definida. Basicamente, os arquivos de teste possuem o nome da função alvo acrescido do nome `.spec.js`.

O arquivo `src/zoo.js` contém a implementação de uma função, `getSpeciesByIds,` por exemplo, e o arquivo `tests/getSpeciesByIds.spec.js` conterá os testes unitários referentes à função.

---

## Desafios

### 1. IMPLEMENTE A FUNÇÃO getSpeciesByIds

  Esta função é responsável pela busca das espécies de animais por id. Ela retorna um array contendo as espécies referentes aos ids passados como parâmetro, podendo receber um ou mais ids.

  **Observações técnicas**

  - O parâmetro desta função pode ser alterado para atender ao requisito proposto

### 2. IMPLEMENTE A FUNÇÃO getAnimalsOlderThan

  Esta função, a partir do nome de uma espécie e uma idade mínima, verifica se todos os animais daquela espécie possuem a idade mínima especificada

  **Observações técnicas**

  - Deve retornar um valor booleano

### 3. IMPLEMENTE A FUNÇÃO getEmployeeByName

   Esta função é responsável pela busca das pessoas colaboradoras através do primeiro ou do último nome delas

### 4. IMPLEMENTE A FUNÇÃO createEmployee

  A função, a partir de informações recebidas nos parâmetros, é capaz de criar um objeto equivalente ao de uma pessoa colaboradora, retornando-o

  **Observações técnicas**

  - O parâmetro `personalInfo` recebe um objeto que contém o `id`, o `firstName` e o `lastName`
  - O parâmetro `associatedWith` recebe um objeto que contém dois array: `managers` e `responsibleFor`

### 5. IMPLEMENTE A FUNÇÃO isManager

  Verifica se uma pessoa colaboradora, a partir de seu id, ocupa cargo de gerência.

  **Observações técnicas**

  - Deve retornar um valor booleano

### 6. IMPLEMENTE A FUNÇÃO addEmployee

  A função irá adicionar uma nova pessoa colaboradora ao array `employees`, presente no arquivo `data.js`.

### 7. IMPLEMENTE A FUNÇÃO countAnimals

  Esta função é responsável por contabilizar a quantidade de animais.

  **Observações técnicas**

  - Sem parâmetros, retorna um objeto
  - Com o nome de uma espécie de animal, retorna um número

### 8. IMPLEMENTE A FUNÇÃO calculateEntry

  A partir da quantidade de visitantes e a faixa etária de cada um, esta função é responsável por retornar o preço total a ser cobrado

  **Observações técnicas**

  - O parâmetro `entrants` recebe um objeto que contém as chaves `Adult`, `Child` e `Senior`, com suas respectivas quantidades de pessoas

### 9. IMPLEMENTE A FUNÇÃO getAnimalMap

  A função é responsável pelo mapeamento geográfico das espécies e seus animais, podendo ainda filtrá-los por ordem alfabética e gênero, por exemplo

  **Observações técnicas**

  - Analise o teste unitário para entender os retornos que são esperados para esta função

### 10. IMPLEMENTE A FUNÇÃO getSchedule

  A função é responsável por disponibilizar as informações de horário para uma consulta, que pode querer ter acesso a todo o cronograma da semana ou apenas o cronograma de um dia específico

  **Observações técnicas**

  - Analise o teste unitário para entender os retornos que são esperados para esta função

### 11. IMPLEMENTE A FUNÇÃO getOldestFromFirstSpecies

  A função busca por informações do animal mais velho da primeira espécie gerenciada pela pessoa colaboradora do parâmetro

### 12. IMPLEMENTE A FUNÇÃO increasePrices

  A função é responsável por aumentar o preço das visitas, com base no valor de aumento recebido no parâmetro, em porcentagem

  **Observações técnicas**

  - Se o parâmetro da função recebe o valor 20, o aumento é de 20%
  - Altera o objeto `prices` do arquivo `data.js`

### 13. IMPLEMENTE A FUNÇÃO getEmployeeCoverage

  A função é responsável por consultar as espécies pela qual a pessoa colaborada, recebida no parâmetro através de seu `id`, `firstName` ou `lastName`, é responsável

  **Observações técnicas**

  - Analise o teste unitário para entender os retornos que são esperados para esta função

---

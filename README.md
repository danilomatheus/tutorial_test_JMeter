<h1 align="left"> Guia de Teste de Stress com o Apache JMeter </h1>

Neste guia irei apresentar como é possível realizar diversos casos de teste de performance utilizando a ferramenta Apache JMeter. Esta ferramenta foi criada no ano de 2007 e ganhou destaque por se tratar de uma ferramenta gratuita e de código aberto, permitindo que a comunidade adapte-a e construa plugins para ambientes diferentes.

# Índice 

* [Título e Imagem de capa](#Título-e-Imagem-de-capa)
* [Badges](#badges)
* [Índice](#índice)
* [Descrição do Projeto](#descrição-do-projeto)
* [Status do Projeto](#status-do-Projeto)
* [Funcionalidades e Demonstração da Aplicação](#funcionalidades-e-demonstração-da-aplicação)
* [Acesso ao Projeto](#acesso-ao-projeto)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Pessoas Contribuidoras](#pessoas-contribuidoras)
* [Pessoas Desenvolvedoras do Projeto](#pessoas-desenvolvedoras)
* [Licença](#licença)
* [Conclusão](#conclusão)

## Requisitos de Instalação (Plataforma Windows)
- [Java(TM) Platform SE binary](https://www.oracle.com/br/java/technologies/downloads//)
- [Apache JMeter](https://jmeter.apache.org/)

## Instalação do JMeter
1. Baixe o arquivo .zip disponível neste [link](https://jmeter.apache.org/) e extraia o mesmo no diretório padrão de _Arquivos de Programa_ do Windows.
2. Dentro da pasta da ferramenta, existe a pasta **bin** onde se encontra o arquivo ApacheJMeter.jar correspondente a ferramenta Desktop que iremos utilizar para realização dos testes. 
3. Contanto que esteja com o Java instalado em sua máquina, execute o ApacheJMeter.jar.

## Exemplo de Teste de Performance em API Rest - Método GET

Para efetuar o teste, iremos fazer uso da API [JSONPlaceholder](https://jsonplaceholder.typicode.com/) que permite a execução de requisições de forma gratuita e sem causar dados a uma aplicação real.

1. Com a aplicação ApacheJMeter em execução salve o plano de testes para que fique registrado o resultado da execução.
2. Clique  com o botão direito em  Plano de Testes/Adicionar/ Threads(Users)/Grupo de Usuários.
3. Em Grupo de Usuários nas propriedades do Usuário Virtual, altere a quantidade de usuários de 1 para 100.
4. Após criar o grupo de usuários, iremos criar uma requisição HTTP. Clique  com o botão direito em Grupo de Usuários/Adicionar/Testador/Requisição HTTP
5. Configure a Requisição em Protocolo [http]: https
6. Por fim, precisamos criar um Ouvinte para que analisemos o resultado da requisição. Para isso, clique  com o botão direito em  Plano de Testes/Adicionar/Ouvinte e escolha a opção Ver Árvore de Resultados.






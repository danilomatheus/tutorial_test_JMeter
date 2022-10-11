<h1 align="left"> Guia de Teste de Performance com o Apache JMeter </h1>

Neste guia irei apresentar como é possível realizar casos de teste de performance utilizando a ferramenta Apache JMeter. Esta ferramenta foi criada no ano de 2007 e ganhou destaque por se tratar de uma ferramenta gratuita e de código aberto, permitindo que a comunidade adapte-a e construa plugins para ambientes diferentes.

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
3. Em Grupo de Usuários nas propriedades do Usuário Virtual, altere a quantidade de usuários de 1 para 100. Dessa forma iremos simular essa quantidade de acessos e 1 a cada segundo.

 ![GroupUsers](https://user-images.githubusercontent.com/13155179/194976631-9d1e9cfb-b3ee-4d37-ab7b-514a52162923.PNG)

4. Após criar o grupo de usuários, iremos criar uma requisição HTTP. Clique  com o botão direito em Grupo de Usuários/Adicionar/Testador/Requisição HTTP
5. Configure a Requisição da seguinte maneira:
 
![requestHttp](https://user-images.githubusercontent.com/13155179/194976561-28b6f3a9-3ad0-4897-bbc4-90ccfd49487d.PNG)

6. Por fim, precisamos criar um Ouvinte para que analisemos o resultado da requisição. Para isso, clique  com o botão direito em  Plano de Testes/Adicionar/Ouvinte e escolha a opção Ver Árvore de Resultados.
7. Se tudo ocorrer conforme esperado, teremos o resultado abaixo:

![resultadoTeste](https://user-images.githubusercontent.com/13155179/194978611-936e2226-c114-4478-8aec-cb56298f180b.PNG)

## Tutorial em Vídeo

[Link](https://drive.google.com/drive/folders/10KZhGCdhxYChsmIeoH7VpBF1C2e0jX0Q?usp=sharing)

## Conclusão
Espero ter contribuído com a comunidade demonstrando esse exemplo de maneira simples e objetiva de utilização da Ferramenta Apache JMeter.






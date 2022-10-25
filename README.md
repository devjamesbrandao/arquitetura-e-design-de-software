<h1 align="center"><strong>Estudos sobre temas diversos de arquitetura e design de software</strong></h1>

### ` 📖 Frases interessantes sobre arquitetura de software`
> "O uso sem necessidade gera complexidade sem sentido"

### ` 📚 Conceitos utilizados em arquitetura de software`
> <strong>OverHead:</strong> pode ser definido como qualquer combinação de tempo de computação excessivo ou indireto, memória, largura de banda, ou outros recursos que são necessários para executar uma tarefa específica. Por exemplo, podemos que dizer que o banco de dados está com overhead quando ele está com um consumo de memória muito alto. <br />

> <strong>Trade-off:</strong> é uma decisão situacional que envolve a diminuição ou perda de uma qualidade, quantidade ou propriedade de um conjunto ou desenho em troca de ganhos noutros aspectos. Por exemplo, se você decide dormir mais tarde para estudar, você está adquirindo mais conhecimento, porém está diminuindo o tempo de descanso (sono).

### ` 📜 Tópicos sobre arquitetura de software`

#### Complexidade
> A <strong>complexidade acidental</strong> é aquela que surge durante o processo de desenvolvimento, ou seja, ela é <strong>CAUSADA</strong> pela abordagem escolhida para resolver o problema. Por exemplo, as vezes o desenvolvedor quer construir uma API no formato de Microsserviço utilizando DDD, CQRS, Event Sourcing, orquestração de container com Kubernetes, etc. Porém, toda essa complexidade é desnecessária, pois o que foi solicitado é apenas uma API CRUD simples. Ou seja, o problema é simples, todavia você está propondo uma solução hiper ultra complexa. <br />
Já a <strong>complexidade essencial</strong> é basicamente a complexidade que nosso <strong>software</strong> se propõe resolver, ou seja, ele é realmente complexo, portanto, exige uma certo nível de complexidade para sua resolução (aqui é onde o filho chora e a mãe não vê).

### PoC (Proof of Concept)
> Prova de Conceito ou PoC, é uma palavra que vem do inglês na qual significa Proof of Concept. Ela busca pela evidência documentada para que um software venha a ser bem-sucedido.
> Por se tratar de um dos primeiros métodos para testar e avaliar uma ideia conceitual para software, produto ou solução para uma empresa, a prova de conceito na prática é como um procedimento cujo o objetivo do mesmo é provar a viabilidade de um conceito e validá-lo em baixa escala.

#### Single Point Of Failure (ponto de falha única)
<p align="center">
    <img src="/img/spof.png" alt="Single Point Of Failure" title="Single Point Of Failure">
</p> 

> <strong>Single Point Of Failure (SPOF)</strong> ou <strong>único ponto de falha</strong> é uma parte de um sistema que, se falhar, impedirá o funcionamento de todo o sistema. Essa abordagem é útil quando temos as responsabilidades da aplicação bem definidas. Nesse sentido, caso haja problemas na aplicação, fica mais fácil de resolver, pois já sabemos, provavelmente, onde está a causa. Por exemplo, digamos que exista uma API desenvolvida em ASP.NET Core que realiza consultas no banco de dados. Para isso, foi criado um repositório responsável por estabelecer conexão com o banco de dados, realizar as consultas solicitadas e devolver os dados. Nesse caso, foi delegado toda a responsabilidade de lidar com o banco de dados para o repositório. Portanto, se houver um problema como, por exemplo, timeout de conexão, é possível concluir que esse problema ocorreu no repositório, visto que a conexão com o banco de dados só ocorre nele. Sendo assim, pode-se dizer que o repositório do exemplo é um SPOF. 

#### Separation Of Concerns
> <strong>Separation of concerns</strong> é um principio de engenharia de software, que visa separar preocupações, ou seja, modularizar aplicação de forma que cada módulo esteja focado em resolver apenas um único problema. Separar preocupações, ou seja, conceitos é imprescindível para quem deseja ter uma arquitetura madura e sustentável. <br />
> Uma das maneiras de se construir um sistema contemplando a separação de conceitos, é separar a sua aplicação em <strong>camadas</strong> e fazer com que cada uma delas foque em resolver tarefas apenas de sua responsabilidade. As camadas, separam conceitos de acordo com a sua função dentro de uma arquitetura. 

<p align="center">
    <img src="/img/soc.png" alt="Exemplo de arquitetura que segue Separation of Concern" title="Exemplo de arquitetura que segue Separation of Concern">
</p> 

#### Princípio Don't Repeat Yourself
> Cada parte do conhecimento deve ter uma <strong>representação única</strong> não ambígua e definitiva dentro da aplicação. Segundo esse princípio, não devemos escrever o mesmo trecho de código em várias partes da aplicação. O ideal seria, de alguma forma, modularizá-lo a fim de reaproveitá-lo.

#### Princípio KISS (Keep It Simple, Stupid)
> O <strong>KISS</strong> valoriza a simplicidade do projeto e defende que toda a complexidade desnecessária seja descartada. De acordo com esse princípio, devemos, sempre que possível, prezar por um código simples e eficiente, sem adicionar complexidade dispensável, como, por exemplo, utilizar arquitetura de Microsserviços para criar uma API CRUD simples. Se não precisa, não faça.

#### Princípio YAGNI (You Ain't Gonna Need It)
> Uma orientação que sugere não adicionar funcionalidades ao código fonte de uma aplicação até que estas sejam realmente necessárias. Ou seja, o desenvolver só deve fazer aquelas funcionalidades solicitadas.

#### Conway's Law
> "Qualquer empresa que projeta um sistema, inevitavelmente produz um projeto cuja estrutura é uma cópia da estrutura de comunicação da organização." - Melvin Conway

### ` 🌐 Referências`
- Amadurecendo com Separation Of Concerns: https://www.devmedia.com.br/amadurecendo-com-separation-of-concerns/18699

- Prova de Conceito (Poc): o que é e como construir?: https://blog.nectarcrm.com.br/o-que-e-prova-de-conceito/


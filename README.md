# sistema bancario com POO

## sobre:
<h4>Meu primeiro projeto sendo desenvolvido com POO (Programação orientada a objetos).
Nesse projeto eu fiz a utilização da linguagem python, que já venho estudando a um tempo e venho me aprimorando.</h4>

## explicação:
<h4>Nesse projeto conta com um sistema de modularização, separando as classes e funcionalidades por arquivos, sendo todos eles executados no main.py.</h4>

### main.py:
<h4>
Este é um arquivo main.py que utiliza os módulos contas, pessoas e banco para criar uma instância do objeto Banco, que contém clientes, contas e agências. O código cria duas instâncias do objeto Cliente, chamados c1 e c2, com os nomes pré-definidos que podem ser trocados. Cada cliente também recebe uma instância de ContaCorrente ou ContaPoupanca, chamados cc1 e cp1, respectivamente.
Em seguida, o código instancia um objeto Banco e adiciona as instâncias de Cliente, ContaCorrente e ContaPoupanca ao banco.
Por fim, o código autentica o Cliente c1 e ContaCorrente cc1 no banco, e se a autenticação for bem-sucedida, o código realiza dois depósitos diferentes na conta de c1, imprimindo o saldo da conta ao final.
</h4>

### banco.py:
<h4>
Este é um arquivo banco.py que define a classe Banco. Essa classe possui métodos para adicionar agências, clientes e contas, além de verificar se um cliente e uma conta são válidos e autenticar um cliente em uma conta. A classe Banco possui três listas: agencias, clientes e contas. Essas listas armazenam instâncias de int, pessoas.Pessoa e contas.Conta, respectivamente.
O método _checa_agencia verifica se a agência de uma conta está na lista de agências do banco. O método _checa_cliente verifica se um cliente está na lista de clientes do banco. O método _checa_conta verifica se uma conta está na lista de contas do banco. E o método _checa_se_conta_e_do_cliente verifica se a conta de um cliente é a mesma que está sendo autenticada.
O método autenticar utiliza esses métodos de checagem para verificar se um cliente pode ser autenticado em uma conta. Se todas as checagens forem bem-sucedidas, o método retorna True. Caso contrário, retorna False.
O método __repr__ é utilizado para retornar uma representação em string da classe Banco.
</h4>

### contas.py:
<h4>
  Este é um simples exemplo de implementação de classes em Python para modelar contas bancárias. O objetivo é fornecer uma estrutura básica que possa ser expandida posteriormente. Conta: classe abstrata que define a estrutura básica de uma conta bancária, com métodos para sacar e depositar dinheiro, bem como para exibir informações sobre a conta.
ContaPoupanca: classe concreta que herda da classe Conta, implementando o método sacar de acordo com as regras de saque de uma conta poupança.
ContaCorrente: classe concreta que herda da classe Conta, implementando o método sacar de acordo com as regras de saque de uma conta corrente, que pode ter um limite de crédito.
As classes ContaPoupanca e ContaCorrente são implementações simples e incompletas de contas bancárias, sem considerar muitas das regras e funcionalidades que existem em sistemas bancários reais. Este código é apenas um exemplo básico para fins educacionais e pode ser usado como ponto de partida para implementações mais complexas.
</h4>


### pessoas.py:
<h4>
pessoas.py é um módulo Python que define duas classes: Pessoa e Cliente. Classe Pessoa
A classe Pessoa é usada para representar uma pessoa com nome e idade. Ela tem dois atributos: nome e idade.

Métodos
A classe Pessoa possui os seguintes métodos:
__init__(self, nome: str, idade: int) -> None: O construtor da classe, que recebe dois parâmetros obrigatórios: nome e idade.
__repr__(self) -> str: Método que retorna uma string representando a instância da classe.
Propriedades: A classe Pessoa define duas propriedades: nome e idade. Elas são usadas para acessar e definir os atributos _nome e _idade, respectivamente.
Classe Cliente: A classe Cliente é uma subclasse de Pessoa que representa um cliente bancário. Além dos atributos nome e idade, um objeto Cliente também tem um atributo conta. Métodos: A classe Cliente não possui métodos próprios, mas herda todos os métodos da classe Pessoa. Propriedades: A classe Cliente define uma propriedade: conta. Ela é usada para acessar e definir o atributo conta, que pode ser uma instância da classe Conta definida em outro módulo.
</h4>

## Obervação:
Sistema feito com o intuito de colocar em pratica os meus o conhecimentos em python em um exercício do curso de python da UDEMY.COM
















# Screen Sound

Bem-vindo ao **Screen Sound**, um console app simples construído em C# para registrar e avaliar suas bandas favoritas.

## 🚀 Funcionalidades

O projeto permite que o usuário interaja com as seguintes opções através de um menu:

1.  **Cadastrar uma banda**: Adiciona um novo nome de banda à lista de bandas registradas.
2.  **Mostrar todas as bandas**: Exibe uma lista de todas as bandas que foram cadastradas.
3.  **Avaliar uma banda**: Permite atribuir uma nota (avaliação) a uma banda existente.
4.  **Mostrar a média de avaliações de uma banda**: Calcula e exibe a média das notas atribuídas a uma banda específica.
5.  **Sair**: Encerra o aplicativo.

## 💻 Como Rodar o Projeto

Este projeto é um aplicativo de console desenvolvido em C#. Para executá-lo, você precisará ter o **.NET SDK** instalado na sua máquina.

1.  **Clone o repositório** (assumindo que o código está em um repositório):

    ```bash
    git clone [LINK_DO_SEU_REPOSITORIO]
    cd ScreenSound
    ```

2.  **Execute o projeto** a partir da pasta raiz do projeto:

    ```bash
    dotnet run
    ```

    O aplicativo será iniciado e o menu de opções será exibido no seu console.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** C#
* **Framework:** .NET (Console Application)

## 📁 Estrutura do Código

O código é implementado em um único arquivo de programa (provavelmente `Program.cs`), utilizando um dicionário (`Dictionary<string, List<int>>`) para armazenar as bandas e suas respectivas notas.

* `bandasRegistradas`: Dicionário onde a `chave` é o nome da banda (`string`) e o `valor` é uma lista de notas (`List<int>`).
* `ExibirOpcoesDoMenu()`: Função principal que exibe o menu e gerencia a navegação entre as funcionalidades.
* `RegistraBanda()`: Lógica para adicionar uma nova banda ao dicionário.
* `MostraBandasRegistradas()`: Lógica para iterar e exibir os nomes das bandas cadastradas.
* `AvaliarUmaBanda()`: Lógica para buscar uma banda e adicionar uma nova nota à sua lista de avaliações.
* `MostraMediaDasBandas()`: Lógica para buscar uma banda, calcular a média das suas avaliações (`.Average()`) e exibi-la.
* `ExibirLogo()` e `ExibirTituloDaOpcao()`: Funções utilitárias para melhorar a experiência visual no console.

## 💡 Exemplos de Uso

Ao iniciar o programa, você verá:

1.  **Cadastrar:** Digite `1`, informe o nome da banda (ex: "Queen").
2.  **Avaliar:** Digite `3`, informe o nome da banda ("Queen"), e depois a nota (ex: `9`).
3.  **Ver Média:** Digite `4`, informe o nome da banda ("Queen"), e veja a média das notas cadastradas.

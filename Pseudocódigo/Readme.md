# Usando Pseudocódigo para Cadastro em uma Agência de Viagens

**Objetivo:** Este pseudocódigo simula um cadastro para uma agência de viagens com as seguintes funções: cadastro de cliente e cadastro de destino. Além disso, é possível consultar os clientes e destinos cadastrados.

Algoritmo AgenciaDeViagens

Função MenuPrincipal()
    Enquanto Verdadeiro
        Escrever("---- Menu Principal ----")
        Escrever("1. Cadastrar Cliente")
        Escrever("2. Cadastrar Destino")
        Escrever("3. Consultar Clientes")
        Escrever("4. Consultar Destinos")
        Escrever("5. Sair")
        Escrever("-------------------------")
        Escrever("Digite a opção desejada: ")
        Ler(opcao)
        
        Se opcao = 1 Então
            CadastrarCliente()
        Senão Se opcao = 2 Então
            CadastrarDestino()
        Senão Se opcao = 3 Então
            ConsultarClientes()
        Senão Se opcao = 4 Então
            ConsultarDestinos()
        Senão Se opcao = 5 Então
            Escrever("Encerrando o programa...")
            Interromper
        Senão
            Escrever("Opção inválida! Digite novamente.")
        Fim Se
    Fim Enquanto
Fim Função

Função CadastrarCliente()
    Escrever("---- Cadastro de Cliente ----")
    Escrever("Digite o nome do cliente: ")
    Ler(nome)
    Escrever("Digite o CPF do cliente: ")
    Ler(cpf)    
   
    Escrever("Cliente cadastrado com sucesso!")
Fim Função

Função CadastrarDestino()
    Escrever("---- Cadastro de Destino ----")
    Escrever("Digite o nome do destino: ")
    Ler(nomeDestino)
    Escrever("Digite a descrição do destino: ")
    Ler(descricao)
    
    Escrever("Destino cadastrado com sucesso!")
Fim Função

Função ConsultarClientes()   
    Escrever("---- Clientes Cadastrados ----")
    Para cada cliente em clientes
        Escrever("Nome: " + cliente.nome)
        Escrever("CPF: " + cliente.cpf)
    Fim Para
Fim Função

Função ConsultarDestinos()   
    Escrever("---- Destinos Cadastrados ----")
    Para cada destino em destinos
        Escrever("Nome do Destino: " + destino.nomeDestino)
        Escrever("Descrição: " + destino.descricao)
    Fim Para
Fim Função

// Início do programa
Função Principal()
    MenuPrincipal()
Fim Função


<p align="center">
  <strong>
    Português
    &nbsp;|&nbsp;
    <a href="./README.en.md">English</a>
  </strong>
</p>

# Sistemas de Gerenciamento Integrados: Clínica Médica, Eventos e Restaurante

## 📌 Descrição do Projeto

Este projeto consiste no desenvolvimento de uma aplicação em **Java**, baseada nos princípios da **Programação Orientada a Objetos (POO)**, que simula **três sistemas de gerenciamento distintos**, integrados em um único sistema:

- 🏥 Clínica Médica  
- 🎟️ Sistema de Eventos  
- 🍽️ Restaurante  

O objetivo principal é aplicar conceitos fundamentais de POO, como **encapsulamento, abstração, modularização e reutilização de código**, além de demonstrar a integração entre diferentes domínios de negócio para **apoio à tomada de decisões estratégicas**.

---

## 👥 Integrantes do Projeto

- Nunno Wakiyama Diniz Carvalho  
- Pedro Henrique Mendes Macedo  
- Ricardo Nery de Brito Junior  
- Matheus Fabiano Barbosa Aguiar  
- **Noemi Soares Gonçalves da Silva**

---

## 🎯 Objetivos

- Aplicar conceitos de Programação Orientada a Objetos em Java  
- Desenvolver sistemas independentes e integrados  
- Simular cenários reais de gestão (saúde, eventos e alimentação)  
- Utilizar dados para responder perguntas estratégicas  
- Desenvolver um sistema modular, extensível e organizado  

---

## 🛠️ Tecnologias Utilizadas

- **Java**
- **Programação Orientada a Objetos**
- **Scanner (entrada de dados via terminal)**
- **Collections (ArrayList)**
- **Estruturas de controle e menus interativos**

---

## 🧩 Estrutura do Sistema

O projeto é dividido em **quatro grandes módulos**:

1. Sistema de Gerenciamento de Clínica Médica  
2. Sistema de Gerenciamento de Eventos  
3. Sistema de Gerenciamento de Restaurante  
4. Sistema Integrado (Tomada de Decisão)

---

## 🏥 Case 1: Sistema de Gerenciamento de Clínica Médica

Este módulo permite:

- Cadastro de médicos e pacientes  
- Agendamento de consultas  
- Verificação de horários ocupados  
- Identificação do médico mais solicitado  

### Principais Classes

- **Clinica**  
  - Classe central do sistema  
  - Gerencia médicos, pacientes e consultas  
  - Métodos principais:
    - `adicionarMedico()`
    - `adicionarPaciente()`
    - `adicionarConsulta()`
    - `medicoMaisSolicitado()`
    - `dataHorariosDeUmMedico()`

- **Paciente**
  - Armazena dados como nome, idade, sintomas, plano de saúde e tipo sanguíneo
  - Métodos getters e setters
  - Método `temPlanoSaude()`

- **Medico**
  - Informações como nome, especialização, CRM e disponibilidade
  - Controle do número de consultas
  - Métodos:
    - `estaDisponivel()`
    - `incrementarContadorDeConsultas()`

- **Consulta**
  - Relaciona médico e paciente
  - Armazena data, horário e prioridade
  - Método `possivelPrioridade()`

---

## 🎟️ Case 2: Sistema de Gerenciamento de Eventos

Este sistema é responsável por:

- Cadastro e gerenciamento de eventos  
- Inscrição de participantes  
- Controle de lotação  
- Geração de relatórios  

### Principais Classes

- **Evento**
  - Gerencia participantes, atrações e capacidade
  - Métodos:
    - `registrarParticipante()`
    - `verificarLotacao()`
    - `gerarRelatorio()`

- **Local**
  - Representa o local do evento
  - Atributos: nome e endereço
  - Sobrescrita do método `toString()`

- **main_event**
  - Interface interativa via terminal
  - Gerencia eventos, participantes e locais
  - Uso intensivo de menus e validações

---

## 🍽️ Case 3: Sistema de Gerenciamento de Restaurante

Sistema voltado para o controle completo de um restaurante:

- Gerenciamento de mesas
- Registro de pedidos
- Controle de itens do cardápio
- Cálculo e fechamento de contas

### Principais Classes

- **Restaurante**
  - Classe central
  - Gerencia até 15 mesas
  - Métodos:
    - `inicializarMesas()`
    - `fazerPedido()`
    - `fecharConta()`

- **Mesa**
  - Representa mesas do restaurante
  - Métodos:
    - `reservar()`
    - `liberar()`

- **ItemDoPedido**
  - Representa itens do cardápio
  - Atributos: nome, preço e tamanho

- **Pedido**
  - Gerencia itens pedidos
  - Métodos:
    - `adicionarItem()`
    - `removerItem()`
    - `calcularTotal()`

---

## 🔗 Case 4: Integração dos Sistemas

A classe **SistemaIntegrado** conecta os três sistemas em um único menu principal, permitindo:

- Acesso unificado aos módulos
- Geração de relatórios
- Respostas a perguntas estratégicas, como:
  - Médico mais solicitado
  - Evento mais popular
  - Prato mais pedido

Essa integração demonstra a aplicação prática de **abstração e reutilização de código**, além de permitir análises mais profundas com base nos dados gerados.

---

## 📊 Tomada de Decisão

O sistema responde perguntas estratégicas baseadas nos dados dos três módulos, auxiliando na análise de desempenho e apoio à tomada de decisões gerenciais.

---

## 📌 Status do Projeto

✅ Projeto finalizado  
📚 Desenvolvido para fins acadêmicos  
🧠 Mantido como material de estudo e portfólio  

---

## 🧾 Conclusão

O projeto resultou em um sistema robusto, modular e integrado, aplicando de forma prática os conceitos de Programação Orientada a Objetos. A divisão clara de responsabilidades entre as classes e a integração entre os módulos proporcionam uma base sólida para futuras expansões, como interfaces gráficas, persistência em banco de dados ou novos módulos de negócio.

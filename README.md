# **React Calculator - Estudo Inicial**

Este projeto é uma **calculadora simples** desenvolvida em **React** como parte do estudo inicial da biblioteca. Ele permite realizar operações matemáticas básicas como soma, subtração, multiplicação e divisão.

## **📜 Descrição do Projeto**
A calculadora foi construída utilizando o **React.js** e demonstra conceitos essenciais como:
- Componentes reutilizáveis (`Button`, `Input`, `Container`, etc.).
- Manipulação de estado com `useState`.
- Gerenciamento de eventos (`onClick` para botões).
- Atualização do estado de forma controlada para garantir operações corretas.

## **🚀 Como Configurar e Executar**

### **1️⃣ Clonar o Repositório**
Antes de começar, certifique-se de ter o **Node.js** instalado na máquina. Clone o projeto via Git:
```bash
git clone https://github.com/seu-usuario/react-calculadora.git


Acesse o diretório do projeto:
cd react-calculadora


2️⃣ Instalar as Dependências
Execute o comando abaixo para instalar todas as dependências necessárias:
npm install


3️⃣ Rodar o Projeto
Agora, execute o comando para iniciar o servidor de desenvolvimento:
npm run start


Após isso, a aplicação estará disponível no navegador no seguinte endereço:
http://localhost:3000


📌 Estrutura do Código
Abaixo está um resumo dos principais arquivos:
react-calculadora/
│── src/
│   ├── components/        # Componentes reutilizáveis
│   │   ├── Button.js      # Botão usado na calculadora
│   │   ├── Input.js       # Campo de exibição de números
│   ├── styles.js          # Estilos da aplicação
│   ├── App.js             # Componente principal
│   ├── index.js           # Ponto de entrada do React
│── package.json           # Dependências do projeto
│── README.md              # Documentação do projeto


🛠️ Como Funciona o Código
O código da calculadora funciona da seguinte forma:
- Gerenciamento de Estado: O estado (useState) armazena os números e operação atual.
- Botões Numéricos: Atualizam currentNumber, permitindo que números sejam digitados.
- Operadores Matemáticos: Definem a operação (+, -, x, /) e armazenam o primeiro número.
- Botão "=": Executa a operação matemática usando um switch, com funções específicas para cada cálculo.
Exemplo da lógica de soma
const handleSumNumbers = () => {
  if (firstNumber === '0') {
    setFirstNumber(currentNumber);
    setCurrentNumber('0');
    setOperation('+');
  } else {
    const sum = Number(firstNumber) + Number(currentNumber);
    setCurrentNumber(String(sum));
    setOperation('');
  }
};


🖥️ Contribuições
Se desejar contribuir com melhorias ou novas funcionalidades, siga os passos:
- Crie uma Branch com sua alteração:
git checkout -b minha-alteracao
- Faça suas alterações e submeta um Pull Request.


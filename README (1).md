# 📊 Sistema de Monitoramento Econômico

Sistema web completo para monitoramento de cotações de moedas em tempo real, consumindo a API pública AwesomeAPI, armazenando histórico em MySQL e exibindo gráficos interativos com alertas personalizáveis.

## 🛠️ Tecnologias Utilizadas

- **Backend:** PHP 8.0+ (PDO, cURL, Programação Orientada a Objetos)
- **Banco de Dados:** MySQL (Hospedado no InfinityFree)
- **Frontend:** HTML5, CSS3, Bootstrap 5, Chart.js
- **IA Copiloto:** Google Gemini
- **Controle de Versão:** Git/GitHub

## 📂 Estrutura do Projeto

```text
projeto-monitoramento/
├── config/
│   ├── database.php          # Conexão PDO com o banco
│   └── database.example.php  # Exemplo de configuração
├── api/
│   └── awesomeapi.php        # Consumo da API externa via cURL
├── models/
│   ├── Cotacao.php           # Model de cotações (CRUD)
│   ├── Alerta.php            # Model de alertas (CRUD)
│   └── Usuario.php           # Model de usuários (Login/Cadastro)
├── controllers/
│   └── CotacaoController.php # Controlador principal
├── public/
│   ├── index.php             # Dashboard principal
│   ├── login.php             # Tela de login
│   ├── cadastro.php          # Tela de cadastro
│   ├── alertas.php           # Gerenciamento de alertas
│   ├── logout.php            # Logout
│   ├── css/style.css         # Estilos personalizados
│   └── js/app.js             # Gráficos Chart.js
├── schema.sql                # Estrutura do banco
├── seed.sql                  # Dados de teste
└── README.md                 # Este arquivo
# RH Project - FrontEnd

Este repositório faz parte do **RH Project**, que é uma aplicação simples para gerenciamento de Recursos Humanos. O projeto é dividido em dois repositórios principais:

- [Backend do RH Project](https://github.com/gabrielandre-math/RH-Project-BackEnd/tree/master)
- [Frontend do RH Project](https://github.com/gabrielandre-math/RH-Project-FrontEnd/tree/master)

Este repositório atual é focado no **Frontend** da aplicação, desenvolvido em **Angular**, e serve como interface para os usuários interagirem com os dados gerenciados pela API do backend.

## Funcionalidades

- Listagem de pessoas, suas informações detalhadas e integração com LinkedIn.
- Paginação para fácil navegação entre as pessoas cadastradas.
- Consumo de uma API FastAPI que entrega dados a partir de uma planilha Excel.
- Interface amigável e responsiva, construída com **Bootstrap** e **Angular Material**.

## Tecnologias Utilizadas

- **Angular**: Framework utilizado para a construção do frontend.
- **Bootstrap**: Para o layout responsivo e estilização dos componentes.
- **Ngx-Pagination**: Biblioteca utilizada para paginação dos dados.
- **Toastr**: Utilizado para notificação de sucesso ou erro nas operações.
- **FastAPI**: API que serve os dados para a aplicação (disponível no repositório backend).
  
## Repositórios do Projeto

1. [Frontend do RH Project](https://github.com/gabrielandre-math/RH-Project-FrontEnd/tree/master)
   
   Contém todo o código da interface da aplicação, responsável por exibir os dados consumidos da API e fornecer uma experiência interativa ao usuário.

2. [Backend do RH Project](https://github.com/gabrielandre-math/RH-Project-BackEnd/tree/master)
   
   A API backend desenvolvida com **FastAPI**, que lida com os dados de uma planilha Excel e os fornece ao frontend para exibição.

## Instalação e Execução do Projeto

### Passos para rodar o Frontend

1. Clone o repositório:
   ```bash
   git clone https://github.com/gabrielandre-math/RH-Project-FrontEnd.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd RH-Project-FrontEnd
   ```

3. Instale as dependências:
   ```bash
   npm install
   ```

4. Inicie o servidor de desenvolvimento:
   ```bash
   ng serve
   ```

5. Acesse o frontend no navegador:
   ```text
   http://localhost:4200
   ```

### Passos para rodar o Backend

1. Clone o repositório:
   ```bash
   git clone https://github.com/gabrielandre-math/RH-Project-BackEnd.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd RH-Project-BackEnd
   ```

3. Crie um ambiente virtual (opcional, mas recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows use: venv\Scripts\activate
   ```

4. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

5. Execute o backend:
   ```bash
   uvicorn main:app --reload
   ```

6. Acesse a API no navegador ou Postman:
   ```text
   http://localhost:8000
   ```

## Estrutura dos Repositórios

### Frontend (Angular)

```text
RH-Project-FrontEnd/
│
├── src/
│   ├── app/
│   │   ├── components/           # Componentes da aplicação
│   │   ├── services/             # Serviços para consumo da API
│   │   └── models/               # Modelos de dados
│   └── assets/                   # Recursos estáticos (imagens, etc)
├── styles.css                    # Estilos globais
├── angular.json                  # Configuração do Angular
└── README.md                     # Documentação do projeto
```

### Backend (FastAPI)

```text
RH-Project-BackEnd/
│
├── main.py                       # Código principal da API FastAPI
├── requirements.txt              # Dependências do projeto
├── nomespessoas.xlsx             # Arquivo Excel com os dados
└── README.md                     # Documentação do projeto
```

## Licença

Este projeto está licenciado sob a licença [MIT](LICENSE).


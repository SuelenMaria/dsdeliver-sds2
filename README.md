# DS Delivery

![DS Delivery](path_to_screenshot.png)

## Descrição

DS Delivery é um sistema completo de entregas, composto por:
- Backend Java Spring Boot
- Frontend web React + TypeScript
- Frontend mobile Expo React Native

O sistema é desenvolvido como projeto acadêmico e suporta gerenciamento de produtos, pedidos e integração com mapas.

## Estrutura do Projeto

- `backend/` - API Java Spring Boot
- `front-web/` - Aplicação web React
- `front-mobile/` - Aplicação mobile Expo React Native

## Funcionalidades

- Cadastro de pedidos e produtos
- Consulta de produtos
- Envio de pedidos para backend
- Interface responsiva para web
- App mobile via Expo
- Uso de mapas para localização de entregas

## Tecnologias Utilizadas

### Backend
- Java 11
- Spring Boot 2.4.2
- Spring Data JPA
- Spring Security
- H2 Database (em memória para desenvolvimento)
- PostgreSQL (dependência de runtime)

### Frontend Web
- React 17
- TypeScript 4.1
- Axios
- React Router DOM v5
- Leaflet / React Leaflet
- React Select
- react-toastify
- react-scripts 5.0.1

### Frontend Mobile
- Expo SDK 41
- React Native 16.13.1
- Axios
- @expo-google-fonts/open-sans
- React Navigation v5

## Requisitos

- Java 11
- Maven (ou use o wrapper `./mvnw` / `.\mvnw.cmd`)
- Node.js 16/18 recomendado
- npm
- Expo CLI local instalada via dependência do projeto

## Instalação e execução

### 1. Clonar o repositório

```bash
git clone https://github.com/seu_usuario/ds-delivery.git
dsdeliver-sds2
```

### 2. Backend

```bash
cd backend
./mvnw spring-boot:run
```

No Windows PowerShell:

```powershell
cd backend
.\mvnw.cmd spring-boot:run
```

A API estará disponível em `http://localhost:8080`.

### 3. Frontend Web

```bash
cd ../front-web
npm install
npm start
```

A aplicação web estará em `http://localhost:3000`.

### 4. Frontend Mobile

```bash
cd ../front-mobile
npm install
npm start
```

Para abrir em Android ou iOS, use:

```bash
npm run android
npm run ios
```

Se o Expo solicitar instalação de `@expo/ngrok`, responda `y`.

## Configuração de ambiente

### Frontend Web
- O frontend web consome a API em `http://localhost:8080` por padrão.
- Para alterar o endpoint, crie um arquivo `front-web/.env` com:

```env
REACT_APP_API_URL=http://localhost:8080
```

### Frontend Mobile
- O mobile consome `process.env.API_URL` se estiver definido.
- Caso contrário, o app usa o backend remoto em `https://suelen-sds2.herokuapp.com`.

## Observações

- O comando `npm start` em `front-web` já define `NODE_OPTIONS=--openssl-legacy-provider` no script de inicialização.
- O `front-mobile` é uma aplicação Expo antiga (SDK 41) e deve ser executado com `npm start` ou `expo start`.

## Desenvolvimento e Git

### Comandos recomendados

```bash
git add README.md
git add front-web/.env
git add front-mobile/package.json
git add front-mobile/package-lock.json
git commit -m "Atualiza README com instruções de execução e setup"
git push origin main
```

### Fluxo de contribuição

1. Crie uma branch de recurso:
   ```bash
   git checkout -b feature/ajuste-readme
   ```
2. Faça alterações e teste localmente.
3. Crie commits claros:
   ```bash
   git commit -m "Atualiza README e instruções de execução"
   ```
4. Envie para o repositório remoto:
   ```bash
   git push origin feature/ajuste-readme
   ```
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT.

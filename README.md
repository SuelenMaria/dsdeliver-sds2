# DS Delivery

![DS Delivery](path_to_screenshot.png)

## Descrição

DS Delivery é um sistema de entregas delivery desenvolvido como projeto acadêmico. Este sistema é projetado para oferecer uma experiência de usuário suave e eficiente tanto em dispositivos desktop quanto móveis.

## Funcionalidades

- **Geolocalização**: Integração com mapas para rastreamento e localização de entregas em tempo real.
- **Temas**: Suporte a temas claro e escuro, permitindo ao usuário escolher a melhor opção de visualização.
- **Versatilidade**: Disponível para desktop e mobile, garantindo acessibilidade e usabilidade em diversas plataformas.

## Tecnologias Utilizadas

### Backend
- **Java**: Linguagem de programação utilizada.
- **SpringTools**: Framework utilizado para criar uma aplicação robusta e escalável.

### Frontend
- **HTML**: Estrutura da aplicação.
- **CSS**: Estilos e design responsivo.
- **TypeScript**: Tipo seguro de JavaScript para melhorar a manutenção e a escalabilidade do código.
- **JavaScript**: Lógica de interação e dinâmica da interface.

## Instalação

### Requisitos
- [Java](https://www.oracle.com/java/technologies/javase-downloads.html)
- [SpringTools](https://spring.io/tools)
- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu_usuario/ds-delivery.git
   ```

2. Navegue até a pasta do backend e inicie a aplicação Spring:
   ```bash
   cd ds-delivery/backend
   ./mvnw spring-boot:run
   ```

3. Navegue até a pasta do frontend e instale as dependências:
   ```bash
   cd ../frontend
   npm install
   ```

4. Inicie a aplicação frontend:
   ```bash
   npm start
   ```

## Uso

1. Acesse a aplicação pelo navegador em `http://localhost:3000`.
2. Navegue pelo sistema utilizando as opções disponíveis.
3. Utilize o mapa para visualizar a localização das entregas.
4. Alterne entre os temas claro e escuro conforme sua preferência.

## Contribuição

1. Faça um fork do projeto.
2. Crie uma nova branch (`git checkout -b feature/nova-feature`).
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`).
4. Envie para o branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

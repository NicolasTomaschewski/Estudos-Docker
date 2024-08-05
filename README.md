## Meus Primeiros Passos com Docker

Neste repositório, compartilho minha experiência inicial com Docker, adquirida durante o curso "Docker: criando e gerenciando containers" da Alura. Como parte do aprendizado, desenvolvi meu primeiro Dockerfile, que permite executar esta aplicação em um container.

### Executando o Projeto

Siga os passos abaixo para rodar o projeto usando Docker:

1. **Criação da Imagem**  
   Primeiro, crie a imagem do container com o seguinte comando:  
   ```bash
   docker build -t nome:versao .
   ```

2. **Execução do Container**  
   Esta aplicação utiliza a porta 3000. Portanto, é necessário mapear essa porta para a porta desejada no host:  
   ```bash
   docker run -d -p porta-desejada:3000 nome:versao
   ```

3. **Acesso ao Projeto**  
   Com o container em execução, o projeto pode ser acessado via navegador em:  
   ```
   http://localhost:porta-desejada
   ```

---

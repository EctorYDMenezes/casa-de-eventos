
# Casa de Eventos

## Descrição
O projeto **Casa de eventos** é uma aplicação para gerenciamento de eventos, que foi containerizada utilizando Docker para facilitar a implantação e execução em diferentes ambientes. A imagem Docker deste projeto está disponível no Docker Hub para ser facilmente baixada e executada.

## Requisitos

- **Docker**: Certifique-se de que o Docker está instalado em sua máquina. [Guia de instalação do Docker](https://docs.docker.com/get-docker/)

## Como baixar e executar a imagem

### 1. Baixar a imagem do Docker Hub

Para baixar a imagem, execute o seguinte comando:
```bash
docker pull ectormenezes/casa-de-eventos
```

### 2. Executar a imagem

Depois de baixar a imagem, você pode executá-la com o seguinte comando:
```bash
docker run -d -p 5173:5173 --name casa-de-eventos ectormenezes/casa-de-eventos
```
Isso irá:
- Executar o container em segundo plano (`-d`).
- Mapear a porta 5173 do container para a porta 5173 da sua máquina local.
- Nomear o container como `casa-de-eventos`.

### 3. Acessar a aplicação

Abra o navegador e acesse [http://localhost:5173](http://localhost:5173) para visualizar a aplicação rodando.

## Testes Locais

### Verificar se o container está em execução
Para garantir que o container está rodando corretamente, use o comando:
```bash
docker ps
```

### Visualizar logs do container (opcional)
Se você quiser verificar os logs da aplicação:
```bash
docker logs casa-de-eventos
```

### Parar e remover o container
Após os testes, você pode parar e remover o container:
```bash
docker stop casa-de-eventos
docker rm casa-de-eventos
```

## Publicação

A imagem do projeto está disponível no Docker Hub. Você pode acessá-la diretamente aqui: [ectormenezes/casa-de-eventos](https://hub.docker.com/r/ectormenezes/casa-de-eventos)

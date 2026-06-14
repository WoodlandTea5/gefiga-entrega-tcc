```markdown
# Manual de Instalação e Execução - GEFIGA

## 1. Pré-requisitos de Ambiente
Para executar o ecossistema Vue.js localmente, certifique-se de ter a ferramenta abaixo instalada em sua máquina:
* **Node.js** (versão 16.x ou superior recomendada): Necessário para o gerenciamento de pacotes (`npm`). Pode ser baixado oficialmente em: https://nodejs.org/

## 2. Instalação das Dependências (Bibliotecas)
Como o arquivo `node_modules` é omitido por boas práticas, você precisará baixar as dependências listadas no `package.json`:
1. Extraia o código-fonte contido nesta pasta `Extras` para um diretório local.
2. Abra o terminal (prompt de comando) e navegue até a pasta raiz do projeto extraído.
3. Execute o comando abaixo para baixar todas as bibliotecas necessárias:
```bash
   npm install

```

## 3. Inicialização e Comunicação com o Firebase

*Nota:* O GEFIGA foi arquitetado no modelo Serverless utilizando o Firebase (Backend-as-a-Service). As chaves de inicialização do SDK (Client Credentials) e as rotas de comunicação com o Cloud Firestore e o Authentication já estão configuradas no código-fonte. Não é necessário levantar um servidor back-end local, pois o front-end fará a ponte direta com a nuvem da Google.

## 4. Executando o Servidor de Desenvolvimento

Com as dependências instaladas, levante o servidor local executando:

```bash
npm run dev

```

*(Caso o projeto utilize versões mais antigas do Vue CLI, o comando equivalente é `npm run serve`).*

O terminal processará os arquivos e exibirá uma porta local (geralmente `http://localhost:5173` ou `http://localhost:8080`). Clique no link exibido no seu terminal para acessar a aplicação funcional pelo navegador.

```

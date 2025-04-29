# Base Repository API

API base construída com [Express.js](https://expressjs.com/) e [TypeScript](https://www.typescriptlang.org/), preparada para escalar com boas práticas de estruturação, testes, validação e configuração de ambiente.

## 📦 Scripts

- `dev` – Inicia o servidor em modo de desenvolvimento com `ts-node-dev`
- `start` – Inicia o servidor em modo de produção com `ts-node`
- `build` – Compila o projeto TypeScript para JavaScript
- `test` – Executa os testes com Jest
- `test:watch` – Executa os testes em modo watch
- `test:cov` – Gera relatório de cobertura de testes
- `test:debug` – Inicia o modo debug para testes
- `crypto` – Script utilitário para criptografia (em `test/utils/crypto.ts`)

## 📚 Dependências

### Produção
- `express` – Framework web
- `zod` – Validação de dados
- `dotenv` – Configuração de variáveis de ambiente
- `bcryptjs`, `jsonwebtoken`, `crypto-js` – Autenticação e criptografia
- `winston` – Logger avançado
- `axios` – Requisições HTTP
- `cors`, `express-async-errors` – Melhorias na API

### Desenvolvimento
- `typescript`, `ts-node-dev`, `ts-jest` – Suporte a TypeScript
- `jest` – Testes unitários
- `eslint`, `prettier` – Padronização de código
- `@types/*` – Tipagens para TypeScript
- `commitlint`, `lint-staged` – Qualidade em commits

## 🚀 Começando

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/base-repository.git
   cd base-repository
   ```

2. Instale as dependências:

    ```bash
    npm install
    Configure o arquivo .env baseado no .env.example (caso exista).
    ```

## Inicie a aplicação:

### Desenvolvimento: 
  ```bash
  pnpm dev
  ```

### Produção: 
 ```bash
  pnpm build && pnpm start
  ```

## 🤝 Como Contribuir
1. Fork este repositório
2. Crie uma branch com sua feature: git checkout -b minha-feature
3. Commit suas alterações: git commit -m 'feat: nova funcionalidade'
4. Push para sua branch: git push origin minha-feature
5. Abra um Pull Request
6. Utilize pnpm lint e pnpm test antes de subir suas mudanças.

## 📄 Licença
Este projeto está licenciado sob os termos da MIT License.

## 🔮 O que está por vir
- Documentação com Swagger
- Integração com banco de dados (Prisma, TypeORM, etc.)
- Autenticação JWT completa
- Estrutura de serviços e repositórios
- Pipeline CI/CD com GitHub Actions
- Deploy automatizado
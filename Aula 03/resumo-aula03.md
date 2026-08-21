# Resumo — Projetos com Frameworks Front-end (Aula 03)

**Professor:** Deivison S. Takatu (SENAI)
**Contato:** deivison.takatu@edu.senai.br

---

## 1. Introdução aos Frameworks Front-end

- Framework: conjunto de ferramentas, bibliotecas e convenções que padronizam o desenvolvimento de interfaces web, acelerando a criação de aplicações complexas.
- **Sem framework (Vanilla JS):** código manual, difícil manutenção, repetição.
- **Com framework:** componentes reutilizáveis, estado gerenciado, atualizações eficientes.

## 2. Framework × Biblioteca

| | Framework | Biblioteca |
|---|---|---|
| Controle | Inversão de controle (o framework decide o fluxo) | Você controla quando chamar |
| Estrutura | Exige estrutura definida | Flexível, sem imposições |
| Exemplos | Angular, Vue | React, jQuery |

**Exemplo prático:**
- Biblioteca: você chama `ReactDOM.render()` quando quiser.
- Framework: o Angular decide quando renderizar os componentes.

## 3. Por que utilizar um framework?

- **Produtividade aumentada:** evita reinventar a roda (roteamento, estado, renderização).
- **Melhores práticas:** código organizado em componentes.
- **Manutenção facilitada:** Virtual DOM (React), Change Detection (Angular).
- **Comunidade e suporte:** documentação extensa, plugins, soluções prontas.

## 4. Principais frameworks/bibliotecas

- **React** — criado pelo Facebook (2013). Tecnicamente é uma **biblioteca**, não um framework. Usa Virtual DOM; exige conhecimento prévio de HTML e JavaScript.
- **Angular** — desenvolvido pelo Google. Framework completo com TypeScript nativo, arquitetura MVC, injeção de dependências e CLI poderosa.
- **Vue.js** — framework progressivo, fácil de adotar gradualmente; usa Single-File Components (`.vue`).
- **Next.js** — framework baseado em React para apps full-stack: roteamento por arquivos, SSR, Server Components, otimização de imagens/fontes, APIs de backend, SEO.

### Comparação entre frameworks (Google Trends / StackShare)
A escolha depende de complexidade do projeto, curva de aprendizado, desempenho e suporte da comunidade. React lidera em popularidade de busca; Angular se destaca por arquitetura robusta e TypeScript nativo.

## 5. Características comuns dos frameworks front-end

- Estrutura de código organizada (separação HTML/CSS/JS)
- Componentização (independência e reutilização)
- Programação reativa (atualização automática da UI)
- Ferramentas de build e bundling (minificação, transpilação)
- Sistema de rotas (SPAs)
- Integração com APIs (chamadas assíncronas, gerenciamento de estado)
- Documentação e comunidade ativas
- Padrões de design e acessibilidade
- Suporte a testes unitários e de integração

## 6. Conceitos fundamentais por tecnologia

**React:**
- Hooks: `useState` (estado), `useEffect` (efeitos colaterais/API)
- JSX: `{}` para expressões, atributos em camelCase (`className`), tags sempre fechadas
- Gerenciamento de estado: Context API (simples) ou Redux (complexo)

**Angular:**
- Componentes com `@Component` (HTML + CSS + TypeScript)
- Módulos (`@NgModule`)
- Serviços com `@Injectable`
- Data binding: `[(ngModel)]` (two-way), `{{ }}` (interpolação)
- Roteamento: `RouterModule`

## 7. Criando projetos (passo a passo)

**Angular:**
```bash
npm install -g @angular/cli
ng new meu-app-angular
cd meu-app-angular
code .
ng serve
```

**Vue:**
```bash
npm create vue@latest
cd meu-projeto-vue
npm install
code .
npm run dev
```

**Next.js:**
```bash
npx create-next-app@latest meu-projeto
cd meu-projeto
code .
npm run dev
```

### Estrutura de pastas (resumo geral)
- `node_modules` — dependências instaladas
- `public` — arquivos estáticos
- `src` / `app` — código-fonte principal (componentes, serviços, módulos)
- Arquivos de config: `angular.json`, `vite.config.js`, `next.config.ts`, `tsconfig.json`, `package.json`, `.gitignore`, `.editorconfig`

## 8. Importando/reaproveitando projetos

Aproveitar projetos open source existentes pode acelerar o desenvolvimento:
- **GitHub** — Repository search (`git clone <url>`)
- **Vercel** — busca por templates (download parcial do repositório)
- **CodeSandbox** — Template Search

## 9. Atividade prática

Desenvolver, **em grupo**, 4 projetos web sobre o mesmo tema, cada um em uma tecnologia:

1. Projeto 01 — **React**
2. Projeto 02 — **Vue**
3. Projeto 03 — **Angular**
4. Projeto 04 — **Next.js**
5. Projeto 05 — cópia de um projeto a partir de um repositório

**Requisitos:**
- Página funcional, responsiva e organizada, usando componentes e recursos básicos de cada tecnologia.
- Versionamento com **Git**, publicado no **GitHub**, com histórico de commits que registre a evolução.
- Ao final, elaborar uma breve comparação entre as quatro tecnologias, destacando as principais diferenças encontradas.

## 10. Referências principais

- SOUZA, Natan. *Bootstrap 4*. Casa do Código, 2018.
- MACHADO, Kheronn Khennedy. *Angular 11 e Firebase*. Casa do Código, 2021.
- EIS, Diego. *Guia Front-end*. Casa do Código, 2015.
- GONÇALVES, Edson. *Desenvolvendo aplicações Web com JSP, Servlets, JSF, Hibernate, EJB 3, Ajax*. Ciência Moderna, 2007.
- HARTCOPP, Patrícia Ferreira. *Métrica Web*. Contentus, 2020.
- NIEDERAUER, Juliano. *Desenvolvendo Websites com PHP*. Novatec, 2017.
- PREECE, ROGERS, SHARP. *Design de Interação*. Bookman, 2013.
- SOUSA, Roque Fernando Marcos. *Canvas HTML 5*. Brasport, 2014.
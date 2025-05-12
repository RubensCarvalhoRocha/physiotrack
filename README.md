# Sistema de Avaliação Fisioterapêutica

Este repositório contém a interface do usuário do sistema de avaliação fisioterapêutica, desenvolvido com **Angular** e **TypeScript** e a API do sistema de avaliação fisioterapêutica, desenvolvida com Spring Boot e Java 17.

## 📌 Objetivo

Permitir que fisioterapeutas cadastrem pacientes, registrem avaliações clínicas, acompanhem a evolução dos pacientes e agendem sessões de forma simples e intuitiva.

## 🚀 Tecnologias Utilizadas

### Frontend

- [Angular 16](https://angular.io/)
- [TypeScript](https://www.typescriptlang.org/)
- [HTML/CSS](https://developer.mozilla.org/)
- [Bootstrap](https://getbootstrap.com/)
- [Node.js](https://nodejs.org/) (ambiente de execução)

### Backend

- [Java 17](https://www.oracle.com/java/)
- [Spring Boot 3](https://spring.io/projects/spring-boot)
- [Maven](https://maven.apache.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Hibernate / JPA](https://hibernate.org/)
- [Spring Security](https://spring.io/projects/spring-security)
- [JWT (JSON Web Token)](https://jwt.io/)
- [Swagger / OpenAPI](https://swagger.io/)
- [Docker](https://www.docker.com/)


## 🛠️ Instalação Front

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/nome-do-repo-frontend.git

# Acesse o diretório
cd nome-do-repo-frontend

# Instale as dependências
npm install

# Rode o servidor de desenvolvimento
ng serve
A aplicação será executada em http://localhost:4200.
```

## 🛠️ Instalação Back
### Backend

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/nome-do-repo-backend.git

# Acesse o diretório
cd nome-do-repo-backend

# Execute a aplicação
./mvnw spring-boot:run

# A aplicação será executada em http://localhost:8080.
```


## 🧪 Testes

```bash
ng test
```

## 🗂️ Estrutura de Pastas do Front:
src/
 └── app/
      ├── components/
      ├── pages/
      ├── services/
      ├── models/
      └── app.module.ts

## 🗂️ Estrutura de Pastas do Back:

src/
 └── main/
      ├── java/
      │    └── com/
      │         └── seuusuario/
      │              └── sistemafisio/
      │                   ├── controller/        # Controladores REST
      │                   ├── service/           # Regras de negócio
      │                   ├── model/             # Entidades JPA
      │                   ├── repository/        # Interfaces de acesso ao banco (Spring Data JPA)
      │                   ├── security/          # Configurações de autenticação e JWT
      │                   └── Application.java   # Classe principal
      └── resources/
           ├── application.yml                  # Configurações da aplicação
           └── static/                          # Recursos estáticos (se necessário)

           
## Plano de Gerenciamento de Configuração

## 1 - Introdução

Este documento tem como objetivo padronizar, orientar e manter o controle sobre os artefatos produzidos durante o desenvolvimento do **Sistema de Avaliação Fisioterapêutica**, estabelecendo diretrizes para controle de versões, políticas de contribuição e práticas de organização de repositórios.

---

## 2 - Itens de Configuração

Neste projeto, os seguintes itens serão considerados como itens de configuração:

- **Código:** arquivos de implementação em Angular (frontend) e Spring Boot (backend).
- **Documentação:** artefatos como requisitos, casos de uso, diagramas, plano de testes, plano de qualidade e cronogramas.
- **Protótipos:** mockups, wireframes e telas desenvolvidas no Figma.
- **Artefatos auxiliares:** planilhas de rastreabilidade, atas, apresentações.

---

## 3 - Ferramentas

| Ferramenta | Uso |
|-----------|-----|
| Git        | Controle de versão do código-fonte |
| GitHub     | Hospedagem dos repositórios, wiki e issues |
| Figma      | Prototipação de telas da interface |
| Google Drive | Armazenamento de artefatos do projeto |
| Visual Studio Code | IDE para desenvolvimento frontend |
| IntelliJ IDEA | IDE para desenvolvimento backend |
| Postman    | Testes de API |
| GitHub Actions | Integração contínua e testes automáticos |

---

## 4 - Repositório de Código

### 4.1 - Política de Commits

- Idioma padrão: **inglês**.
- Mensagens de commit devem ser claras, objetivas e começar com verbo no infinitivo.
- Exemplo: `Add endpoint to register new patient`.
- Commits conjuntos devem conter a assinatura de todos os autores com `--author` ou `-s`.

### 4.2 - Política de Branches

- `main`: versão estável (produção).
- `dev`: versão de desenvolvimento integrada.
- Branches de funcionalidade, correção ou documentação devem ser criadas a partir de `dev`.

### 4.3 - Padrões para Criação e Uso das Branches

- Casos de Uso: `UC_RegisterPatient`
- Histórias de Usuário: `US_PatientCanViewReport`
- Correções e Configurações: `FIX_LoginBug`
- Issues: `ISSUE_15_RemoveDeprecatedEndpoint`

### 4.4 - Política de Aprovação

- Todo `Pull Request` deve:
  - Ser revisado por outro membro da equipe (Arthur, Bruno ou Rubens).
  - Passar por build e testes automáticos (GitHub Actions).
  - Estar vinculado a uma issue ou funcionalidade registrada.

### 4.5 - Versionamento de Código

- Segue o padrão [Semantic Versioning 2.0.0](https://semver.org/):
  - **MAJOR**: mudanças incompatíveis.
  - **MINOR**: novas funcionalidades compatíveis.
  - **PATCH**: correções de bugs e ajustes menores.

---

## 5 - Repositório de Documentação

- A documentação será armazenada na Wiki e no [Google Drive do Projeto](https://drive.google.com/drive/folders/1mNhX4d9eKeUskvX0J3QhObBBZ3vB4RHx?usp=sharing).
- Arquivos devem ser nomeados com padrão claro, indicando a versão se necessário.

### 5.1 - Versionamento de Documentos

- Segue a convenção **MAJOR.MINOR**.
  - Exemplo: `1.2` indica segunda revisão menor do documento principal.
  - Atualizações pequenas (ortografia, estilo) → MINOR.
  - Mudanças estruturais ou conteúdo novo → MAJOR.

---

## 6 - Monitoramento e Controle

A gerência do projeto (Arthur Luz) é responsável por fiscalizar a aplicação dos padrões definidos neste plano. Cabe à gerência:

- Validar merges e estrutura de branches.
- Garantir que os documentos estejam organizados e versionados.
- Auxiliar membros da equipe com dúvidas sobre as práticas de configuração.

---

##👨‍💻 Contribuidores

Arthur Luz – Gerente de Projeto

Bruno – Desenvolvedor Full Stack

Rubens – Desenvolvedor Full Stack


## 7 - Referências

- PMI. Um Guia do Conhecimento em Gerenciamento de Projetos – PMBOK® 5ª ed.
- [Semantic Versioning 2.0.0](https://semver.org/)
- Exemplo de Plano de Configuração: [PlataformaJogosUnB](https://github.com/fga-gpp-mds/2017.1-PlataformaJogosUnB/wiki/Plano-de-Gerenciamento-de-Configura%C3%A7%C3%A3o-de-Software)





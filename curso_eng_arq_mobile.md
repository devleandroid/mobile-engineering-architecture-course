# 📱 Formação Avançada: Engenharia & Arquitetura de Software Mobile (Android & Swift)

Bem-vindo ao repositório oficial do programa de especialização em **Engenharia e Arquitetura de Software Mobile**. Este repositório foi estruturado no formato de plataforma aberta (*self-paced*), onde todo o conteúdo técnico, materiais complementares em PDF e especificações de projetos estão organizados em diretórios.

---

## 🗂️ Estrutura do Repositório

```text
.
├── 📄 README.md
├── 📄 CERTIFICATION.md
├── 📁 01-engenharia-de-software-mobile/
│   ├── 📁 modulo-01-fundamentos-e-qualidade/
│   │   ├── 📄 README.md
│   │   ├── 📁 docs/ (Guias em PDF)
│   │   └── 📁 projeto-pratico/
│   ├── 📁 modulo-02-testes-automatizados/
│   │   ├── 📄 README.md
│   │   ├── 📁 docs/ (Guias em PDF)
│   │   └── 📁 projeto-pratico/
│   └── 📁 modulo-03-devops-e-observabilidade/
│       ├── 📄 README.md
│       ├── 📁 docs/ (Scripts e Guias)
│       └── 📁 projeto-pratico/
└── 📁 02-arquitetura-de-software-mobile/
    ├── 📁 modulo-01-padroes-arquiteturais-e-ui/
    │   ├── 📄 README.md
    │   ├── 📁 docs/ (Diagramas e PDFs)
    │   └── 📁 projeto-pratico/
    ├── 📁 modulo-02-modularizacao-e-di/
    │   ├── 📄 README.md
    │   ├── 📁 docs/ (Boilerplates e PDFs)
    │   └── 📁 projeto-pratico/
    └── 📁 modulo-03-performance-seguranca-capstone/
        ├── 📄 README.md
        ├── 📁 docs/ (Templates de ADR)
        └── 📁 projeto-pratico/
```

---

# 🚀 Especialidade 1: Engenharia de Software Mobile

---

## 📂 `01-engenharia-de-software-mobile/modulo-01-fundamentos-e-qualidade`

### 📺 Vídeo-Aulas Recomendadas
*   [Android Developers - Kotlin Coroutines & Flow Deep Dive](https://www.youtube.com/watch?v=fSB6_KE95bU)
*   [Apple Developer - Swift Concurrency (Async/Await & Actors)](https://developer.apple.com/videos/play/wwdc2021/10132/)
*   [Refactoring Guru - SOLID Principles & Design Patterns in Mobile](https://www.youtube.com/results?search_query=solid+principles+mobile)

### 📄 Materiais de Apoio (Download)
*   [📥 Manual_de_Code_Review_e_Estilo.pdf](./docs/Manual_de_Code_Review_e_Estilo.pdf)
*   [📥 Cheatsheet_Gerenciamento_de_Memoria.pdf](./docs/Cheatsheet_Gerenciamento_de_Memoria.pdf)

### 🛠️ Projeto Prático do Módulo 1: Refatoração de App Legado
*   **Objetivo:** Receber um projeto legadomente acoplado com vazamentos de memória e sem assincronismo moderno.
*   **Requisitos:**
    1. Identificar e eliminar no mínimo 2 *memory leaks* (Retain Cycles / Static Contexts) com suporte de profiling.
    2. Migrar o código de requisições assíncronas para **Kotlin Coroutines/Flow** (Android) ou **Swift Concurrency async/await** (iOS).
    3. Aplicar os princípios **SOLID** na camada de dados e negócios.
*   **Entrega:** Submeter Pull Request na pasta `projeto-pratico/` contendo o relatório de vazamentos corrigidos.

---

## 📂 `01-engenharia-de-software-mobile/modulo-02-testes-automatizados`

### 📺 Vídeo-Aulas Recomendadas
*   [Android Developers - Testing in Jetpack Compose](https://www.youtube.com/watch?v=P_J34u9I9-w)
*   [WWDC - Meet Swift Testing & Modern XCUITest Integration](https://developer.apple.com/videos/play/wwdc2024/10179/)
*   [Philipp Lackner - MockWebServer & Integration Testing in Android](https://www.youtube.com/watch?v=J_3qT_Rll7M)

### 📄 Materiais de Apoio (Download)
*   [📥 Ebook_Estrategias_de_Mocks_Stubs_e_Fakes.pdf](./docs/Ebook_Estrategias_de_Mocks_Stubs_e_Fakes.pdf)
*   [📥 Template_Suite_de_Testes_Starter_Kit.zip](./docs/Template_Suite_de_Testes_Starter_Kit.zip)

### 🛠️ Projeto Prático do Módulo 2: Suíte de Testes E2E (E-Commerce)
*   **Objetivo:** Criar a cobertura de testes automatizados para um fluxo completo de checkout de e-commerce.
*   **Requisitos:**
    1. Escrever testes unitários cobrindo as regras de negócio de cálculo de frete e desconto.
    2. Implementar testes de integração simulando respostas de rede com **MockWebServer** (Android) ou **URLProtocol** (iOS).
    3. Criar testes de interface/UI reativa garantindo a navegação no fluxo de pagamento.
    4. Atingir no mínimo **80% de cobertura de código**.
*   **Entrega:** Submeter repositório no módulo com o relatório de cobertura gerado via JaCoCo ou Xcode Coverage.

---

## 📂 `01-engenharia-de-software-mobile/modulo-03-devops-e-observabilidade`

### 📺 Vídeo-Aulas Recomendadas
*   [Fastlane Docs - Automated Build and Release for iOS and Android](https://www.youtube.com/watch?v=wXm9pB2cOvw)
*   [GitHub Actions - CI/CD Workflow for Android & Swift](https://www.youtube.com/watch?v=R8_veQiYGio)
*   [Firebase Crashlytics & Sentry Best Practices](https://www.youtube.com/watch?v=k_0Z_k3U26g)

### 📄 Materiais de Apoio (Download)
*   [📥 Fastfile_and_Github_Actions_Templates.zip](./docs/Fastfile_and_Github_Actions_Templates.zip)
*   [📥 Checklist_Publicacao_PlayStore_AppStore.pdf](./docs/Checklist_Publicacao_PlayStore_AppStore.pdf)

### 🛠️ Projeto Prático do Módulo 3: Esteira CI/CD Automatizada
*   **Objetivo:** Configurar uma esteira de integração e entrega contínua end-to-end.
*   **Requisitos:**
    1. Criar um arquivo `.github/workflows/main.yml` configurado para executar compilação, linters e testes a cada Pull Request.
    2. Configurar scripts do **Fastlane** para geração automática de build assinada.
    3. Automatizar a distribuição para o **Firebase App Distribution** ou **TestFlight** na mesclagem para a branch `main`.
*   **Entrega:** Link do Pull Request com a execução bem-sucedida do Action e comprovante da build gerada no painel de distribuição.

---

# 🏛️ Especialidade 2: Arquitetura de Software Mobile

---

## 📂 `02-arquitetura-de-software-mobile/modulo-01-padroes-arquiteturais-e-ui`

### 📺 Vídeo-Aulas Recomendadas
*   [Android Developers - Guide to App Architecture (Clean Arch + UDF)](https://www.youtube.com/watch?v=p1hC9_L8_y4)
*   [SwiftUI & Modern Architecture - Point-Free Unidirectional Data Flow](https://www.youtube.com/watch?v=0_u_S0K_E3Y)
*   [Reso Coder - Clean Architecture Concepts](https://www.youtube.com/watch?v=KwhR17S_S-k)

### 📄 Materiais de Apoio (Download)
*   [📥 Diagramas_Arquitetura_Clean_UDF.drawio](./docs/Diagramas_Arquitetura_Clean_UDF.drawio)
*   [📥 Core_Architecture_Base_Project.zip](./docs/Core_Architecture_Base_Project.zip)

### 🛠️ Projeto Prático do Módulo 1: Core Architecture App (Finanças)
*   **Objetivo:** Estruturar a arquitetura base de um aplicativo financeiro altamente escalável.
*   **Requisitos:**
    1. Implementar arquitetura baseada em **Clean Architecture** dividida em camadas transparentes (Domain, Data, Presentation).
    2. Utilizar **Unidirectional Data Flow (UDF)** no gerenciamento de estado com Jetpack Compose ou SwiftUI.
    3. Garantir o desacoplamento total da camada Domain em relação a frameworks de UI e redes externos.
*   **Entrega:** Código-fonte publicado na pasta do módulo com documentação da árvore de pacotes e estado da UI.

---

## 📂 `02-arquitetura-de-software-mobile/modulo-02-modularizacao-e-di`

### 📺 Vídeo-Aulas Recomendadas
*   [Android Developers - Modularization Strategies for Scale](https://www.youtube.com/watch?v=1M0m_fS6k9E)
*   [Krzysztof Zabłocki - iOS Architecture at Scale & SPM Modules](https://www.youtube.com/watch?v=8V9x9Vz5bJg)
*   [Philipp Lackner - Dependency Injection with Hilt / Swinject Deep Dive](https://www.youtube.com/watch?v=bbMsuI2p1XA)

### 📄 Materiais de Apoio (Download)
*   [📥 Guia_Matriz_de_Dependencias_e_Build_Times.pdf](./docs/Guia_Matriz_de_Dependencias_e_Build_Times.pdf)
*   [📥 Multi_Module_Boilerplate_Gradle_SPM.zip](./docs/Multi_Module_Boilerplate_Gradle_SPM.zip)

### 🛠️ Projeto Prático do Módulo 2: Refatoração para Multi-Módulos
*   **Objetivo:** Transformar um app monolítico em uma estrutura modular por funcionalidades (*Feature Modules*).
*   **Requisitos:**
    1. Isolar componentes reutilizáveis em um módulo `:core` ou `CorePackage`.
    2. Separar telas ou fluxos em módulos independentes (`:feature:auth`, `:feature:dashboard`).
    3. Configurar **Injeção de Dependências (Hilt/Koin ou Swinject)** gerenciando escopos entre os módulos.
    4. Configurar navegação desacoplada através de *Router Pattern* ou *Coordinators*.
*   **Entrega:** Pull Request exibindo a matriz de dependências limpa e relatório demonstrando a redução no tempo de build incremental.

---

## 📂 `02-arquitetura-de-software-mobile/modulo-03-performance-seguranca-capstone`

### 📺 Vídeo-Aulas Recomendadas
*   [Android Studio Profiler - Analyzing Memory, CPU & Rendering Issues](https://www.youtube.com/watch?v=3W8mYc7A3nU)
*   [WWDC - Modern iOS Security: Keychain, Certificate Pinning & Privacy](https://developer.apple.com/videos/play/wwdc2020/10688/)
*   [Software Architecture - Writing Architectural Decision Records (ADRs)](https://www.youtube.com/watch?v=N4X5bO1fS80)

### 📄 Materiais de Apoio (Download)
*   [📥 Template_Oficial_ADR_C4_Model.docx](./docs/Template_Oficial_ADR_C4_Model.docx)
*   [📥 Checklist_Auditoria_de_Seguranca_Mobile.pdf](./docs/Checklist_Auditoria_de_Seguranca_Mobile.pdf)

### 🏆 Projeto Capstone Final: Enterprise Architecture & Security
*   **Objetivo:** Projetar e construir um aplicativo de grande escala focado em mercado financeiro ou saúde, cobrindo todos os pilares do curso.
*   **Requisitos:**
    1. **Documentação Técnica:** Redação de 2 **ADRs (Architecture Decision Records)** e diagramas no padrão **C4 Model** (Contexto e Contêineres).
    2. **Segurança:** Implementação de **Certificate Pinning**, armazenamento seguro via Android Keystore/iOS Keychain e ofuscação de código (ProGuard/R8 ou Swift Shield).
    3. **Performance:** Submissão de relatórios do Profiler demonstrando 0 *jank frames* e ausência de vazamento de memória sob carga.
    4. **Modularização & Testes:** Projeto multi-módulo integrado com cobertura de testes mínima de 80%.
*   **Entrega:** Submissão do repositório final e abertura de Issue no repositório principal solicitando a banca de avaliação do time de mentores.

---

## 🎓 Avaliação e Emissão de Certificados

Para verificar os requisitos de aprovação automatizada via GitHub Actions e solicitar a emissão do certificado assinado, acesse o documento [CERTIFICATION.md](./CERTIFICATION.md).
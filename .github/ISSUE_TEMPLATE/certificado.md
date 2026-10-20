name: 🎓 Solicitação de Certificado
description: Utilize este template para solicitar a emissão do seu certificado de conclusão.
title: "[SOLICITAÇÃO DE CERTIFICADO] - <Seu Nome Completo>"
labels: ["certificação", "avaliação"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        ## 📜 Requisitos de Certificação
        Antes de enviar, certifique-se de que:
        - [ ] Seu repositório está **público** no GitHub.
        - [ ] Todas as pipelines do GitHub Actions estão passando (status verde).
        - [ ] O Projeto Capstone foi avaliado e aprovado (nota ≥ 8.0) por um mentor.

  - type: input
    id: nome_completo
    attributes:
      label: Nome Completo (como deve aparecer no certificado)
      description: "Ex: João da Silva"
      placeholder: "Seu nome completo"
    validations:
      required: true

  - type: input
    id: repo_link
    attributes:
      label: Link do Repositório Principal
      description: "URL do seu repositório no GitHub contendo todas as entregas."
      placeholder: "https://github.com/seu-usuario/seu-repo"
    validations:
      required: true

  - type: textarea
    id: prs_modulos
    attributes:
      label: Links dos Pull Requests Aprovados (por Módulo)
      description: "Cole os links dos PRs aprovados de cada módulo concluído."
      placeholder: |
        - Módulo 1 (Engenharia): [Link do PR]
        - Módulo 2 (Engenharia): [Link do PR]
        - Módulo 1 (Arquitetura): [Link do PR]
        ...
    validations:
      required: true

  - type: input
    id: capstone_eval
    attributes:
      label: Link da Avaliação do Projeto Capstone
      description: "Link da Issue ou PR onde o mentor deixou a aprovação e nota ≥ 8.0."
      placeholder: "https://github.com/devleandroid/mobile-engineering-architecture-course/issues/..."
    validations:
      required: true

  - type: checkboxes
    id: checklist
    attributes:
      label: Confirmação
      options:
        - label: "Confirmo que li o [CERTIFICATION.md](./CERTIFICATION.md) e atendo a todos os requisitos."
          required: true
        - label: "Confirmo que o código é de minha autoria e está pronto para Code Review final."
          required: true

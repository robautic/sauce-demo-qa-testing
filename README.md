# Sauce Demo — Projeto de Testes Manuais

Projeto de testes manuais desenvolvido como parte do portfólio 
de Quality Assurance (QA).

O sistema testado é o [Sauce Demo](https://www.saucedemo.com), 
uma aplicação web de e-commerce criada especificamente para 
prática de testes de software.

---

## Objetivo

Planejar, documentar e executar testes manuais cobrindo os 
principais fluxos funcionais da aplicação, aplicando boas 
práticas de QA como rastreabilidade, documentação de evidências 
e registro de bugs.

---

## Estrutura do Projeto
sauce-demo-qa-testing/

├── testes_manuais_saucedemo.xlsx   # Planilha principal do projeto

└── evidencias/                      # Screenshots dos testes executados

### Abas da Planilha

| Aba | Descrição |
|-----|-----------|
| **Test Plan** | Planejamento geral, escopo e abordagem de testes |
| **Cenários** | 28 cenários mapeados por módulo |
| **Casos de Teste** | 31 casos de teste detalhados com passos e resultados |
| **Bug Report** | 4 bugs documentados com severidade e evidências |
| **Massa de Dados** | Credenciais e dados utilizados na execução |
| **Relatório Final** | Consolidação dos resultados da execução |

---

## Módulos Testados

- **Login** — Fluxos de autenticação (válido, inválido, bloqueado, campos vazios)
- **Produtos** — Listagem, ordenação, detalhes, adição ao carrinho
- **Carrinho** — Adição, remoção e navegação
- **Checkout** — Preenchimento de formulário, validações e finalização de compra

---

## Resultado da Execução

| Módulo | Total | Passaram | Falharam |
|--------|-------|----------|----------|
| Login | 6 | 6 | 0 |
| Produtos | 12 | 9 | 3 |
| Carrinho | 6 | 6 | 0 |
| Checkout | 7 | 7 | 0 |
| **Total** | **31** | **28** | **3** |

Taxa de aprovação: 90,3%

---

## Bugs Encontrados

Todos os bugs foram encontrados utilizando o usuário `problem_user`.

| ID | Título | Severidade | Status |
|----|--------|------------|--------|
| BUG02 | Imagens repetidas em todos os produtos | Média | Aberto |
| BUG03 | Botão "Remove" sem efeito na página de produtos | Alta | Aberto |
| BUG04 | "Add to cart" sem efeito em 3 produtos específicos | Crítica | Aberto |
| BUG05 | Filtro de ordenação completamente inoperante | Alta | Aberto |

---

## Ferramentas Utilizadas

- **Planilha:** Microsoft Excel
- **Versionamento:** Git + GitHub
- **Ambiente de testes:** Google Chrome
- **Gestão de evidências:** Screenshots organizados por caso de teste

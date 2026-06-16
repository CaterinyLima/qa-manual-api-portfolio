# Caso de Teste: CT-009 - Vunerabilidade Login com injecção de script

## Descrição 
Garantir que a aplicação sabe lidar corretamente com dados inválidos, inesperados ou maliciosos, sem quebrar ou expor o sistema.

---

## Informações Gerais
| Campo | Definição|
| :--- | :--- | 
| **Funcionalidade:** | Login |
| **Tipo de Teste:** | Segurança |
| **Prioridade:** | Alta |
| **Ambiente:** | Staging |

---

## Pré-condições
1. O navegador web deve estar aberto na página de login do sistema.

## Dados do Teste (Massa de Dados)
* **Usuário:** `<script>alert('Vulneravel')</script>`
* **Senha:** `123456`

---

## Passos de Execução & Resultados

| Passo | Ação do usuário | Resultado Esperado |
| :--- | :--- | :--- |
| **01** | Introduzir exatamente o seguinte texto `<script>alert('Vulneravel')</script>` no campo "Username". | O texto é inserido corretamente. |
| **02** | Inserir a senha `123456` no campo "Password". | A senha é inserida e mascarada por segurança (ex:••••••). |
| **03** | Clicar no botão "login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username and password do not match any user in this service`. |

---

## Pós-condição
* O utilizador permanece retido  na tela de login (acesso não autorizado).
* [Ver evidência](./evidencias/CT-009-login-vinerabilidade-injecçao-script.png)
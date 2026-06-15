# Caso de teste: CT-005 - Login com senha incorreta.

## Descrição
Garantir que o sistema impeça o login e exiba uma mensagem de alerta quando o formulario for submetido com a senha incorreta.

---

## Informações Gerais

| Campo | Definições |
| :--- | :--- |
| **Funcionalidade** | Login |
| **Tipo de teste** | Negativo |
| **Prioridade** | Alta |
| **Ambiente** | Staging |

---

## Pré-condições 
1. O utilizador deve estar previamente registrado e com a conta ativa na base de dados.
2. O navegador web deve estar aberto na página de login do sistema.

## Dados do teste (Mesa de Dados)
* **Usuário:** `standard_user`
* **Senha** `secretsauce_`

---

## Passos da Execução & Resultados

| Passo | Ação do usuário | Resultado Esperado |
| :--- | :--- | :--- |
| **01** | Introduzir o utilizador `standard_user` no campo "Username". | O utilizador é inserido corretamente. |
| **02** | Inserir a senha `secretsauce_` no campo "Password". | A senha é inserida e mascarada por segurança (ex:••••••••). |
| **03** | Clicar no botão "Login". | O sistema barra o acesso e exibe a mensagem: `Epic sadface: Username and password do not match any user in this service`. |

---

## Pós-condição
* O utilizador permanece retido na tela de login (Acesso não autorizado).
* [Ver evidencia](./evidencias/CT-005-login-senha-invalida.png)
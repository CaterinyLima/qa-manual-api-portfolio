# 🧪 Caso de Teste: CT-001 - Login com credenciais válidas

## 📝 Descrição
Validar se o utilizador consegue autenticar-se com sucesso no sistema ao introduzir um nome de utilizador e uma palavra passe válida, sendo direcionado para a página principal.

---

## ⚙️ Informações Gerais

| Campo | Definição |
| :--- | :--- |
| **Funcionalidade** | Autenticação de usuário / Login |
| **Tipo de Teste** | Positivo |
| **Prioridade** | Alta |
| **Ambiente** | Staging |

---

## 🔍 Pré-condições
1. O utilizador deve estar previamente registrado e com a conta ativa na base de dados.
2. o navegador web deve estar aberto na página de login do sistema.

## 📊 Dados de Teste (Massa de Dados)
* **Username:** `standard_user`
* **Password:** `secret_sauce`

---

## 🛠️ Passos de Execução & Resultados

| Passo | Ação do Usuário | Resultado Esperado |
| :---: | :--- | :--- |
| **01** | Introduzir utilizador `standard_user` no campo "Username" | O utilizador é inserido corretamente |
| **02** | Inserir a senha 'secret_sauce' no campo "password" | a senha é inserida mascarada por segurança (ex: ••••••••). |
| **03** | clicar no botão "Login" | O sistema processa a operação, valida dos dados e redireciona o utilizador para a pagina principal. |

---

## 🏁 Pós-condições
 * Usuário logado com sucesso!
 [Ver Evidência](./evidencias/test-cases/CT-001-Login-Sucesso-01.png)  
 (./evidencias/test-cases/CT-001-Login-Sucesso-02.png)

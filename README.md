# Atividade

## 🔍 Onde localizar os códigos desenvolvidos?

Para facilitar a correção e avaliação da atividade, os arquivos modificados e criados estão distribuídos nas seguintes pastas do projeto:

* **Model (Estrutura de Dados & Validação):**
  * `Atividade/Models/Aluno.cs` — Contém a classe `Aluno` com os atributos decorados com as regras de validação (`[Required]`, `[EmailAddress]`, `[StringLength]`).

* **Controller (Regras de Negócio & Rotas):**
  * `Atividade/Controllers/AlunoController.cs` — Gerencia as requisições `[HttpGet]` e `[HttpPost]` para o carregamento do formulário, validação do `ModelState` e redirecionamento de sucesso.

* **Views (Interface de Usuário em HTML/Razor):**
  * `Atividade/Views/Aluno/Cadastrar.cshtml` — Tela que renderiza o formulário de cadastro utilizando os *Tag Helpers* (`asp-for`).
  * `Atividade/Views/Aluno/Confirmacao.cshtml` — Tela de sucesso (alerta verde) que exibe dinamicamente os dados populados do aluno cadastrado.

---

## 🚀 Como testar localmente?

Ao executar a aplicação (seja pelo VS Code ou Visual Studio), acesse a URL base do seu servidor local adicionando a rota do formulário:

```http
https://localhost:PORTA/Aluno/Cadastrar

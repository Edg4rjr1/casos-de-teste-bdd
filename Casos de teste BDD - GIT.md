**#01 - Criar nova conta de cliente**

|Cenário:|**CT01- Criar nova conta com credencias válidas**|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de Criar uma nova conta</p><p></p><p></p>|
|BDD|<p>Dado que insiro dados válidos nos campos obrigatórios</p><p></p><p>Quando clico no botão Criar uma nova conta.</p><p></p><p>Então exibe a mensagem "Obrigado por registrar sua conta"</p>|
|Resultado esperado:|<p>O usuário deve ser redirecionado para a página "Minha conta" e ter acesso aos outros recursos do sistema.</p><p></p>|

|Cenário:|**CT02 - Criar nova conta com caracter especial no nome**|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de criar uma nova conta.</p><p></p>|
|BDD|<p>Dado que preencho os campos de Informações Pessoais com algum caracter especial.</p><p></p><p>Quando clico no botão Criar uma conta.</p><p></p><p>Então exibe uma mensagem de "Nome inválido"</p><p></p>|
|Resultado esperado:|O usuário deve permanecer na página e o campo inválido deve ser destacado, exibindo a mensagem de erro correspondente.|

|Cenário:|**CT03 - Criar conta sem @ no e-mail**|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de criar uma nova conta e já ter preenchido os campos de Informações Pessoais.</p><p></p>|
|BDD|<p>Dado que insiro um e-mail sem o @ (edgar10hotmail.com)</p><p></p><p>Quando clico no botão Criar uma conta.</p><p></p><p>Então exibe a mensagem "Insira um endereço de e-mail válido (Ex.: johndoe@domain.com)"</p>|
|Resultado esperado:|<p>O usuário deve permanecer na página de criação de conta e a mensagem de erro deve ser exibida.</p><p></p>|

|Cenário:|**CT04 - Criar nova conta com e-mail já cadastrado.**|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|Alta|
|Pré- condições:|Estar na página de criar uma nova conta e já ter preenchido os campos de Informações Pessoais e inserir um e-mail que já está cadastrado no sistema.|
|BDD|<p>Dado que insiro um email já existente no sistema.</p><p></p><p>Quando clico em Criar nova conta.</p><p></p><p>Então exibe a mensagem "Já existe uma conta cadastrada com esse e-mail"</p>|
|Resultado esperado:|O usuário deve permanecer na mesma página e a mensagem de erro deve ser exibida.|

|Cenário:|<p>**CT05- Criar nova conta que a senha tenha menos de 8 caracteres.**</p><p></p>|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alto</p><p></p>|
|Pré- condições:|Estar na página de criar uma nova conta e já ter preenchidos os campos obrigatórios.|
|BDD|<p>Dado que insiro uma senha com número de caracteres inferior a 8.</p><p></p><p>Quando clico no botão de login.</p><p></p><p>Então exibe a mensagem "A senha deve ter 8 ou mais caracteres."</p>|
|Resultado esperado:|O usuário deve permanecer na mesma página e a mensagem de erro deve ser exibida.|

**#02 - Login**

|Cenário:|<p>**CT05- Login com credenciais válidas.**</p><p></p>|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de login.</p><p></p>|
|BDD|<p>Dado que insiro dados válidos nos campos de e-mail ou senha.</p><p></p><p>Quando clico no botão de Login.</p><p></p><p>Então exibe a mensagem "Você efetuou o login"</p>|
|Resultado esperado:|Usuário deve ser redirecionado para a página home e ter acesso as funcionalidades do sistema.|

|Cenário:|<p>**CT06- Login com credenciais inválidas.**</p><p></p>|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de login.</p><p></p>|
|BDD|<p>Dado que insiro dados inválidos nos campos de e-mail ou senha.</p><p></p><p>Quando clico no botão de Login.</p><p></p><p>Então exibe a mensagem "O login da conta está incorreto ou sua conta está desativada"</p>|
|Resultado esperado:|<p>O usuário deve permanecer na página de login e a mensagem de erro deve ser exibida.</p><p></p>|

|Cenário:|<p>**CT07- Login com o campo e-mail sem @**</p><p></p>|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Alta</p><p></p>|
|Pré- condições:|<p>Estar na página de login.</p><p></p>|
|BDD|<p>Dado que insiro um e-mail sem @ e uma senha válida.</p><p></p><p>Quando clico no botão de login.</p><p></p><p>Então exibe a mensagem "Insira um e-mail válido"</p>|
|Resultado esperado:|O usuário deve permanecer na página e o campo inválido deve ser destacado, exibindo a mensagem de erro correspondente.|

|Cenário:|<p>**CT08- Login sem preencher nenhum campo.**</p><p></p>|
| :- | :- |
|Status do Teste:|<p>Aprovado</p><p></p>|
|Prioridade:|<p>Baixo</p><p></p>|
|Pré- condições:|<p>Estar na página de Login.</p><p></p>|
|BDD|<p>Dado que não insiro nenhum simbolo nos campos email e senha.</p><p></p><p>Quando clico no botão de login.</p><p></p><p>Então deve ser exibida a mensagem "Preencha os campos obrigatórios"</p>|
|Resultado esperado:|O usuário deve permanecer na página de login e os campos que não foram preenchidos devem ficar destacados.|


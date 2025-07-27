# 📘 Desafio Criativo TDS Company
> Os emojis possuem significado positivo/atenção/negativo quanto a avaliação após os testes  
![Site utilizado no desafio](https://www.automationexercise.com/)
---  

### Cenário de teste - Cadastro:  
🚀 Feature: Cadastro de Usuário  
              > Sendo um usuário interessado em comprar na plataforma  
              > Quero realizar meu cadastro e acessá-la  
              > Para escolher meus produtos de interesse e comprá-los  

🧪 Cenário:  Página de Cadastro  
              > Dado que sou Usuário, estou na Página Home  
              > Quando clico em “Signup / Login” localizado no Menu Fixo à cima  
              > Então é listada a opção de "New User Signup!" para preenchimento dos campos de "Name" e "Email Address", após clicar no botão "Signup"   
              > E consigo realizar o preenchimento do formulário para cadastro, com os seguintes campos: "Title", "Name*", "Email*", "Password*", "Date of Birth", "First name*", "Last name*", "Company", "Address*", "Address 2", "Country*", "State*", "City*", "Zipcode*", "Mobile Number*"


✅ Fluxo principal de sucesso: cadastrar os dados com sucesso.  
✅ Fluxo principal de insucesso: cadastrar dados previamente cadastrados.  
✅ Fluxo alternativo de sucesso: encaminhamento de login após realizar o cadastro.  
✅ Fluxo alternativo de insucesso: inserir um tipo que não seja email(sem o padrão "nome@dominio.com").  
🧐 Fluxo alternativo de sucesso: os campos condizem com sua obrigatoriedade.
> ⚠️ Sugestão de melhoria identificada(usabilidade): ao submeter o formulário em branco o front indicar abaixo de cada campo que é necessário seu preenchimento pela obrigatoriedade indicada (asterisco). Ou o back juntamente enviar um pop-up contendo a informação que ainda há campos a serem preenchidos.  
> ⚠️ Sugestão de ajuste: as apis utilizadas do fonts google estão reclamando de algumas fontes (GET http://fonts.googleapis.com/css?family=Roboto:400,300,400italic,500,700,100), identificado no inspecionar > network/console.

---
### Cenário de teste - Login:   
🚀 Feature: Login de Usuário     
              > Sendo um usuário já cadastrado na plataforma     
              > Quero realizar meu login     
              > Para acessar a plataforma de compras online    

🧪 Cenário:  Página de Login  
              > Dado que sou Usuário, estou na Página Home   
              > Quando clico em “Signup / Login” localizado no Menu Fixo à cima    
              > Então é listada a opção de "Login to your account" para preenchimento dos campos de "Email Address" e "Password", após clicar no botão "Login"   
              > E consigo acessar e realizar compras na plataforma   

✅ Fluxo principal de sucesso: realizar login com sucesso com uma conta já previamente cadastrada.  
✅ Fluxo principal de insucesso: realizar login com uma conta inexistente em sua base de dados.  
✅ Fluxo alternativo de insucesso: login incorreto e senha correta, não sendo possível logar.  
✅ Fluxo alternativo de insucesso: login correto e senha incorreta, não sendo possível logar.  


---  
### Cenário de teste - Processo de compras na plataforma:
🚀 Feature: Realizar compras no na plataforma     
              > Sendo um usuário já logado na plataforma     
              > Quero realizar meu processo de busca    
              > Para escolher meus produtos de interesse e comprá-los     

🧪 Cenário:  Adicionar produtos ao carrinho  
              > Dado que sou Usuário, estou na Página Home   
              > Quando clico em “Products” localizado no Menu Fixo à cima    
              > Então é listadas as opções de compras    
              > E consigo adicionar ao carrinho ao clicar na opção "Add to cart"   

🧪 Cenário:  Finalizar compra  
              > Dado que sou Usuário, estou na Página Home   
              > Quando clico em “Cart” localizado no Menu Fixo à cima    
              > Então é listadas os produtos adiconados ao carrinho    
              > E ao clicar no botão "Place Order" consigo preencher os seguintes campos para finalizar a compra: "Name on Card", "Card Number", "CVC" e "Expiration", logo após clicar no botão "Pay and Confirm Order".   
            

✅ Fluxo principal de sucesso: procurar item de compra de interesse > entrar em detalhes do produto > adicionar ao carrinho > finalizar a compra.  
✅ Fluxo principal de insucesso: escolher os produtos > inseri-los no carrinho > acessar o carrinho > finalizar a compra não preenchendo os dados do cartão de crédito.   
✅ Fluxo alternativo de insucesso: escolher os produtos > inseri-los no carrinho > acessar o carrinho > finalizar a compra > sem estar logado.  
🧐 Fluxo alternativo de sucesso: filtrar a busca por categoria/marcas > encontrar os itens desejados > adicioná-los ao carrinho > encerrar a compra com o pagamento.   
> ⚠️ Sugestão de melhoria(usabilidade): indicativo visual de onde está a categoria/marca filtrada, mesmo havendo o título, seria útil que estivesse com uma cor mais intensa na opção escolhida.

❌ Fluxo alternativo de insucesso: inserir caracteres não condizentes ao tipo do campo no formulário de pagamento.  
> ⚠️ Os campos de “CVC” e “Expiration” são do tipo number e aceitaram letras, assim como ultrapassaram a quantidade indicada e mesmo assim permite a finalização do processo de pagamento.  



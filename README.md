# 📘 Desafio Criativo TDS Company

![Site utilizado no desafio](https://www.automationexercise.com/)

### Cenário de teste - Cadastro:

✅ Fluxo principal de sucesso: cadastrar os dados com sucesso.  
✅ Fluxo principal de insucesso: cadastrar dados previamente cadastrados.  
✅ Fluxo alternativo de sucesso: encaminhamento de login após realizar o cadastro.  
🧐 Fluxo alternativo de sucesso: os campos condizem com sua obrigatoriedade.
> ⚠️ Sugestão de melhoria identificada(usabilidade): ao submeter o formulário em branco o front indicar abaixo de cada campo que é necessário seu preenchimento pela obrigatoriedade indicada (asterisco). Ou o back juntamente enviar um pop-up contendo a informação que ainda há campos a serem preenchidos.  
> ⚠️ Sugestão de ajuste: as apis utilizadas do fonts google e de alguma imagem que deveria ter carrregado estão com erros identificados no inspecionar > console.  

### Cenário de teste - Login:

✅ Fluxo principal de sucesso: realizar login com sucesso com uma conta já previamente cadastrada.  
✅ Fluxo principal de insucesso: realizar login com uma conta inexistente em sua base de dados.  
✅ Fluxo alternativo de insucesso: login incorreto e senha correta, não sendo possível logar.  
✅ Fluxo alternativo de insucesso: login correto e senha incorreta, não sendo possível logar.  

### Cenário de teste - Processo de compras no site:

✅ Fluxo principal de sucesso: procurar item de compra de interesse > entrar em detalhes do produto > adicionar ao carrinho > finalizar a compra.  
✅ Fluxo principal de insucesso: escolher os produtos > inseri-los no carrinho > finalizar a compra não preenchendo os dados do cartão de crédito.  
🧐 Fluxo alternativo de sucesso: filtrar a busca por categoria/marcas > encontrar os itens desejados > adicioná-los ao carrinho > encerrar a compra com o pagamento.  
> ⚠️ Sugestão de melhoria(usabilidade): indicativo visual de onde está a categoria/marca filtrada, mesmo havendo o título, seria útil que estivesse com uma cor mais intensa na opção escolhida.

❌ Fluxo alternativo de insucesso: inserir caracteres não condizentes ao tipo do campo.  
> ⚠️ Os campos de “CVC” e “Expiration” são do tipo number e aceitaram letras, assim como ultrapassaram a quantidade indicada.  



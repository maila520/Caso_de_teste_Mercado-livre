# 🧪 Caso de Teste - Site Mercado Livre (Estudo Pessoal)

## Funcionalidade Principal: Barra de Pesquisa

### 🎯 Cenário 1 - Verificar se o fluxo principal (barra de pesquisa) está funcionando corretamente  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o usuário esteja na tela principal  
**E:** Clica no campo de pesquisa  
**Quando:** Ele digita "Televisão"  
**Então:** Somente produtos relacionados a televisores devem aparecer.  
**Resultado Obtido:** O sistema retornou produtos relacionados a televisores, incluindo televisões e acessórios compatíveis, conforme esperado.  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 2 - Aplicar um filtro mais refinado (Televisão Samsung)  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o usuário esteja na tela principal  
**Quando:** Buscar na barra de pesquisa por "Televisão Samsung"  
**Então:** Deve retornar somente televisores da marca Samsung.  
**Resultado Obtido:** Retornou apenas televisores da marca Samsung.  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 3 - Aplicar um filtro mais refinado (Televisão Samsung 32 polegadas)  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o usuário esteja na página principal  
**Quando:** No campo de pesquisa, ele digita "Televisão Samsung 32 polegadas"  
**Então:** O resultado deverá retornar somente televisores da marca Samsung de 32 polegadas.  
**Resultado Obtido:** Retornou televisores da marca Samsung com 32 polegadas.  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 4 - Pesquisa por código de produto (SKU: un32t4300agxzd)  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente esteja na página principal  
**Quando:** Busca na barra de pesquisa pelo código SKU "un32t4300agxzd"  
**Então:** Deve retornar somente a televisão Samsung Smart TV 32".  
**Resultado Obtido:** Retornou corretamente a Smart TV Samsung 32".  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 5 - Pesquisa com emoji (📺 Televisão)  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o usuário esteja na tela principal e com pressa  
**Quando:** O usuário digita o emoji 📺 no campo de pesquisa  
**Então:** O sistema deve exibir a mensagem de erro: “Não há anúncios que correspondam à sua busca.”  
**Resultado Obtido:** A mensagem de erro foi exibida corretamente.  
**Status:** ✅ Aprovado  

---

## 🔄 Fluxo Alternativo - Testando os Filtros

### 🎯 Cenário 6 - Teste de filtro por marca específica  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente entrou na página principal  
**E:** Pesquisou por "Televisão"  
**Quando:** Filtrou a marca LG  
**Então:** Deve retornar apenas televisores da marca LG.  
**Resultado Obtido:** Retornou corretamente televisores da marca LG.  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 7 - Teste de filtro por maior preço  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente entrou na página principal  
**E:** Pesquisou por "Mesa de 4 cadeiras"  
**Quando:** Filtrou por “Maior preço”  
**Então:** Deve retornar mesas de 4 cadeiras com os valores mais altos.  
**Resultado Obtido:** A listagem apresentou corretamente os produtos de maior preço.  
**Status:** ✅ Aprovado  

---

### 🎯 Cenário 8 - Teste de filtragem avançada (Sofá)  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente entrou na página principal  
**E:** Buscou no campo de pesquisa por "Sofá"  
**Quando:** Filtrou por sofá de 3 lugares, novo e da cor preta  
**Então:** Deve retornar apenas sofás com 3 lugares, pretos e novos.  
**Resultado Obtido:** Retornou sofá de 3 lugares, novo, porém não apenas da cor preta na página 1.  
**Status:** ❌ Reprovado  

---

### 🎯 Cenário 9 - Teste de filtro por Frete Grátis  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente entrou na página principal  
**E:** Buscou no campo de pesquisa por "Sofá"  
**Quando:** Filtrou por "Frete Grátis"  
**Então:** Deve retornar apenas sofás com frete gratuito.  
**Resultado Obtido:** Um sofá que cobrava frete no valor de 3820,00R$ na página 1.  
**Descrição:** Sofá Retrátil Reclinável 3 Lugares C Molas 1,80m Vegas Suede Cor Preto.
**Status:** ❌ Reprovado  

---

### 🎯 Cenário 10 - Teste de filtro por valor menor que R$1500,00  
**Pré-condição:** Usuário já está logado  

**Dado:** Que o cliente entrou na página principal  
**E:** Buscou no campo de pesquisa por "Sofá"  
**Quando:** Filtrou pela condição de preço menor que R$1500,00  
**Então:** Deve retornar sofás abaixo de R$1500,00.  
**Resultado Obtido:** Retornou corretamente produtos abaixo de R$1500,00.  
**Status:** ✅ Aprovado  

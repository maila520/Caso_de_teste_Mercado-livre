## Caso de Teste - site Mercado Livre ( para meu proprio estudo)

## Funcionalidade (fluxo principal) :

**Cenario verificar se o fluxo principal (barra de pesquisa) está funcionando corretamente**
pré condição : Usuario já está logado

Dado: que o usuario está na tela principal 
E: clica no campo de pequise
Quando: ele escreve para pesquisar por Televisão 
Então: Somente produtos relacionados a televisores devem aparecer.
Resultado Obtido: O sistema retornou produtos relacionados a televisores, incluindo televisões e acessórios compatíveis, conforme esperado.

**Aplicar um filtro mais refinado no fluxo principal**
pré condição : Usuario já está logado

Dado: que o usuario esteja na tela principal 
Quando: buscar na barra de pesquisa, por Televisão Samsung 
Então: Deve retornar somente Televisão da marca Samsung  

**Aplicar um filtro mais refinado no fluxo principal**
pré condição : Usuario já está logado

Dado: que o usuario esteja na pagina principal 
Quando: no campo de presquisa ele escrever Televisão Samsung 32 polegadas
Então: Resultado deverá retornar somente Televisão da marca Samsung tendo 32 polegadas

**Pesquisa por código de produto (SKU-un32t4300agxzd)**
pré condição : Usuario já está logado

Dado: que o cliente esteja na pagina principal
Quando: busca na barra de pesquisa pelo codigo SKU un32t4300agxzd
Então: deve retornar somente televisão Samsung Smart TV 32"


**Pesquisa por emogi mais o nome assim:📺 televisão**

Dado: Dado que o usuario que esteja na tela principal e com pressa 
Quando: o usuario colocar o emoji 📺 
Então: mensagem de erro escrito: Não há anúncios que correspondam à sua busca











**Cenario Verificar se o Fluxo alternative dentro do principal está funcionando**


# dio-lab-azuresearch

Neste laboratório nós criamos um índice de busca Azure AI Search para uma rede de cafés. 
Tivemos que criar um Azure AI Search, Azure AI service e uma conta de Storage no Azure.

![Resources](/prints/resources.png?raw=true "Resources")

Utilizamos o resource grup RG-azureai-search para deixar separado todos os recursos que são utilizados neste laboratório e ter uma ideia do custo.
Todos os recursos foram criado no East-US e a Storage account como Locally redundant (redundante apenas localmente) para deixar um custo mais baixo.

![Storage](/prints/storage.png?raw=true "Storage")

Fizemos o upload dos documentos de resenha dos cafés para o Storage da Azure para que possam ser processados (indexados) pelo mecanismo do Azure AI search. 

![Reviews](/prints/reviews.png?raw=true "Reviews")

A configuração da indexação e o enriquecimento (através do Cognitive Skill do Azure AI Service) é realizado no Import Data do Azure AI Search. Nessa tela, também criamos um indexador que realiza o trabalho propriamente dito.

Por fim, podemos fazer uma consulta no índice criado:

![Consulta](/prints/consulta.png?raw=true "Consulta")


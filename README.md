
# Laboratório AI Search Azure

Esse projeto está baseado na inteligência de Documentos do AI Azure, soluções de pesquisa cognitiva.

## Primeiros Passos 🚶🏼‍♀️

Inicialmente iremos criar uma conta no **Azure AI Services|AI Search** no  [Portal Azure](https://portal.azure.com/#view/Microsoft_Azure_ProjectOxford/CognitiveServicesHub/~/overview) conforme abaixo:

![AI-SEARCH](https://github.com/Jessyfran/SEARCH_AI/blob/main/ContaAISearch.png?raw=true)

**OBS.:** *Alterar o tipo de preço para "BASIC" no momento da criação da conta de teste.*

- Próximo é criar um recurso **Azure AI Services** adicionando o Standard f0 conforme as documentações.

![Services](https://github.com/Jessyfran/SEARCH_AI/blob/main/CriarRecursoServices.png?raw=true)

- Criar também no portal do Azure uma **conta de Armazenamento** (Storage Accounts) para armazenar os arquivos na Azure. Adicionar o *LSR* no recurso para armazenamento simples.

![StorageAccount](https://github.com/Jessyfran/SEARCH_AI/blob/main/StorageAccounts.png?raw=true)


## Configurações de Pesquisa ⚙ 
Para realização do Laboratório será necessário *permitir acesso anônimo ao Blob*, pois nas ações futuras irá ser necessário alterar um container de armazenamento. Para isso, basta entrar no storage account criado e ir em configurações na tela do lado esquerdo conforme a imagem abaixo:

![Configurações](https://github.com/Jessyfran/SEARCH_AI/blob/main/Configura%C3%A7%C3%B5es.png?raw=true)

## Adicionando os arquivos na conta de armazenamento 📥

No Storage Account (conta de armazenamento) terá uma opção de container no lado esquerdo da tela:

![Container](https://github.com/Jessyfran/SEARCH_AI/blob/main/containers.png?raw=true)


Após ter sido criado os containers é hora de fazer o upload dos arquivos baixados na documentação da Azure (Downloads teste Azure), esses arquivos são os dados para as pesquisas testes a serem realizadas. 

![Upload](https://github.com/Jessyfran/SEARCH_AI/blob/main/Upload.png?raw=true)


## Iniciando a Pesquisa 🔎

Após seguir o passo a passo também disponível na documentação (Fundamentos AI Search) é hora de utilizar as pesquisas na ferramenta.
Os arquivos pesquisados são da própria documentação da Azure.
Primeiramente na página do serviço de pesquisa em *visão geral* vá em SEARCH EXPLORER para iniciar suas pesquisas e ver o resultados de forma mais prática.

![Explorador de pesquisa](https://github.com/Jessyfran/SEARCH_AI/blob/main/Explorador%20de%20pesquisa.png?raw=true)

Você pode utilizar a pesquisa em modo Json conforme a documentação ou com o comandos abaixo:

```
search=sentiment:'negative'
search=locations:'Chicago'
```

No caso esses exemplos são devido aos arquivos no qual adicionamos no container. Os arquivos contem informações das avaliações dos clientes numa rede de cafeteria contendo palavras-chave como: Sentimentos, localização, entre outros. Dessa forma o *search* é a inicial da pesquisa, logo após o tipo de palavra-chave seguido em aspas simples('') o resultado que queremos filtrar.

![Exemplo de pesquisa](https://github.com/Jessyfran/SEARCH_AI/blob/main/Exemplo%20de%20pesquisa.png?raw=true)


## 📚Documentação

[Fundamentos AI Search](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

[GitHub-ajuda](https://github.com/Jessyfran/SEARCH_AI.git)

[Downloads teste Azure](https://aka.ms/mslearn-coffee-reviews)


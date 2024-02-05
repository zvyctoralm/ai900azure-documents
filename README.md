# ai900azure-documents
Para realizar o uso da ferramenta de AI Search, o passo a passo é:
1. Vá até portal.azure.com
2. Clique em "Create a resource"
3. Crie um novo Search Service com a opção de "Pricing Tier" como "Basic". 
4. Crie um novo recurso "Azure AI Services"
5. Preencha os dados necessários;
6. Após isso, clique um "Storage Account" > Create
7. Preencha as informações, sabendo que o campo de "Performance" como "Standard" e o campo "Redundancy" como "Locally-redudant storage".
8. OBS: Colocar sempre a região como EAST US por questões de custos.
9. Clique em "Configuration" na aba esquerda e coloque a opção "Allow Blob annonymous acess" como Enabled e Salve.
10. Vá até Containers e crie um novo Container com o nome "coffeereviews".
11. Clique no Container e clique em "Upload". Faça o upload dos arquivos que podem ser baixados na documentação (https://aka.ms/km-documents)
12. Vá até Azure Search novamente e clique em "Import data".
13. Clique em Coonect to your data e selecione "Azure Blob Storage". 
14. Preencha os dados necessários e clique em "Next: Add cognitive skills". 
15. Na aba de Attach Cognitive Services, na parte "Add enrichments" mude o "Skillset name" para "coffee-skillset". 
16. Selecione o checkbox "Enable OCR andmerge all text into merged_content field". 
17. Selecione "Enrichment granularity level" para "Pages (5000 character chunks)".
18. Preencha as informações faltantes.
19. Selecione "Next: create an indexer" e troque o nome para "coffee-indexer".
20. Troque "Schedule" para "Once" e expanda as opções avançadas.
21. Verifique se "Base-64 Encode Keys" está selecionada".
22. Clique em "Submit" e na página Overview, selecione a a aba de Indexers. 

Esse tipo serviço é bastante importante na área de conferência fiscal, no qual, quando por exemplo há vários vendedores (em uma empresa de fertilizantes) que necessitam realizar visitas a clientes, o gasto com alimentação e hospedagem é alto. Consequentemente, a quantidade de notas fiscais é grande, tornando o processo de conferência e inserção no sistema lento. O reconhecimento desses documentos maximiza a produtividade e diminui o texto gasto com esses lançamentos.
Outra aplicação é no arquivamente de notas fisicas nos servidores sem que seja necessário escanear nota por nota. 

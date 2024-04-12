# Azure-Cognitive-Search-andoAISearchparaindexa-oeconsultadeDados
Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados
**Guia Prático: Criando um Índice do Azure AI Search para a Fourth Coffee**

**Objetivo:**
Este guia prático tem como objetivo ajudar você a criar um índice do Azure AI Search para a Fourth Coffee, uma rede nacional de cafés, que permitirá a mineração de conhecimento para facilitar a busca de insights sobre as experiências dos clientes.

**Passo 1: Criar Recursos do Azure**

1. Entre no portal do Azure.
2. Clique no botão "+ Criar um recurso" e pesquise "Azure AI Search".
3. Crie um recurso Azure AI Search com as seguintes configurações:
   - Assinatura: Sua assinatura do Azure.
   - Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo.
   - Nome do serviço: Um nome exclusivo.
   - Localização: Escolha qualquer região disponível.
   - Nível de preços: Básico.
4. Após a validação, selecione "Create".

**Passo 2: Criar Recurso de Serviços de IA do Azure**

1. Na página inicial do portal do Azure, clique em "+ Criar um recurso" e pesquise "Serviços de IA do Azure".
2. Selecione "Criar um plano de serviços de IA do Azure".
3. Configure-o com as mesmas configurações do recurso do Azure AI Search.
4. Após a validação, selecione "Create".

**Passo 3: Criar uma Conta de Armazenamento**

1. Retorne à página inicial do portal do Azure e selecione "+ Criar um recurso".
2. Procure "Conta de Armazenamento" e crie um recurso com as configurações necessárias.
3. Após a validação, aguarde a conclusão da implantação.

**Passo 4: Carregar Documentos para o Armazenamento do Azure**

1. Na conta de armazenamento criada, habilite o acesso anônimo de Blob.
2. Na seção "Containers", crie um contêiner com o nome "Coffee-Reviews" e nível de acesso público como "Container".
3. Baixe as avaliações de café compactadas e extraia os arquivos para a pasta de avaliações.
4. No portal do Azure, selecione o contêiner "Coffee-Reviews" e faça o upload dos arquivos.

**Passo 5: Indexar os Documentos**

1. No portal do Azure, navegue até o recurso Azure AI Search e selecione "Importar dados".
2. Escolha "Azure Blob Storage" como fonte de dados e preencha os detalhes.
3. Anexe o recurso de serviços de IA do Azure e adicione habilidades cognitivas.
4. Personalize o índice de destino e crie um indexador.
5. Aguarde até que o indexador seja executado com sucesso.

**Passo 6: Consultar o Índice**

1. Utilize o Search Explorer na página Visão geral do serviço de pesquisa.
2. Escreva e teste consultas para validar a qualidade do índice de pesquisa.
3. Explore diferentes consultas para filtrar e analisar os resultados.

**Passo 7: Revisar o Armazenamento de Conhecimento**

1. Volte à conta de armazenamento do Azure e navegue até o contêiner de armazenamento de conhecimento.
2. Visualize os dados enriquecidos extraídos pelas habilidades de IA, como projeções e tabelas.
3. Explore as frases-chave e outras informações relevantes capturadas durante o processo de indexação.

Com este guia, você criou com sucesso um índice do Azure AI Search para a Fourth Coffee, permitindo a busca eficiente de insights sobre as experiências dos clientes a partir dos dados de avaliações de café.

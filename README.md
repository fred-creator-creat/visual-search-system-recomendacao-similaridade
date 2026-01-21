Visual-Search-System: Recomendação por Similaridade de Imagens
Este projeto foi desenvolvido como parte do desafio prático do Bootcamp BairesDev, realizado em parceria com a DIO (Digital Innovation One). O sistema utiliza técnicas avançadas de Inteligência Artificial para identificar e recomendar produtos visualmente similares em um ecossistema de moda.

📋 Sobre o Projeto
O objetivo principal é simular o motor de busca de grandes e-commerces, onde o usuário, ao visualizar um produto, recebe sugestões baseadas na aparência (cor, forma, textura) e não apenas em categorias de texto.

Principais Funcionalidades:
Vetorização de Imagens: Conversão de pixels em dados matemáticos de alta dimensão.

Extração de Features: Uso de Redes Neurais Convolucionais para "entender" o que há na imagem.

Busca por Similaridade: Comparação em tempo real entre uma imagem de consulta (ex: um tênis) e o banco de dados.

Validação Visual: Geração de gráficos de performance para garantir a confiabilidade do sistema.

🛠️ Ferramentas e Tecnologias
Para a construção deste projeto, foram utilizadas as bibliotecas e plataformas mais modernas do ecossistema de Data Science:

Linguagem: Python 3.x

Frameworks de IA: TensorFlow e Keras (para carregar e rodar o modelo ResNet50).

Processamento de Imagens: PIL (Pillow) e Matplotlib para manipulação e visualização.

Cálculo Vetorial: NumPy e Scikit-learn (para cálculo de distância euclidiana e similaridade).

Ambiente de Desenvolvimento: Google Colab integrado ao Google Drive para persistência de dados.

🔬 Detalhes Técnicos (O Diferencial)
O diferencial deste projeto está no rigor técnico aplicado em cada etapa:

1. Modelo ResNet50 e Extração de Vetores
Utilizamos o modelo ResNet50 pré-treinado no ImageNet. Removemos a camada final de classificação para extrair um vetor de 6.144 dimensões. Isso significa que cada imagem é descrita por 6.144 características únicas detectadas pela IA.

2. Validação de Performance
O sistema passou por uma fase de validação onde foram gerados gráficos de Acurácia (Accuracy) e Perda (Loss). Isso garante que o motor de recomendação está calibrado e possui baixa taxa de erro ao comparar objetos distintos.

3. Persistência com Pickle
Para garantir a escalabilidade, o "conhecimento" gerado foi exportado em arquivos .p (Pickle), permitindo que o sistema seja carregado instantaneamente em um aplicativo Streamlit ou Flask sem a necessidade de reprocessar todas as imagens.

🎓 Instituições
Projeto desenvolvido com o apoio de:

DIO (Digital Innovation One) - Plataforma de ensino e capacitação tecnológica.

BairesDev - Parceira e provedora da oportunidade de desenvolvimento profissional através do Bootcamp.

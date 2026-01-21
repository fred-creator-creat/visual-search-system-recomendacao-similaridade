# 🚀 Visual-Search-System: Recomendação por Similaridade de Imagens

Este projeto foi desenvolvido como parte do desafio prático do **Bootcamp BairesDev**, realizado em parceria com a **DIO (Digital Innovation One)**. O sistema utiliza técnicas avançadas de **Inteligência Artificial** para identificar e recomendar produtos visualmente similares em um ecossistema de moda.

---

## 📋 Sobre o Projeto

O objetivo principal é simular o motor de busca de grandes e-commerces. Através deste sistema, ao visualizar um produto, o usuário recebe sugestões baseadas na **aparência física (cor, forma, textura)** e não apenas em categorias de texto simples.

### **Principais Funcionalidades:**
* **Vetorização de Imagens:** Conversão de pixels em dados matemáticos de alta dimensão.
* **Feature Extraction (ResNet50):** Uso de Redes Neurais Convolucionais para "entender" o conteúdo visual.
* **Busca por Similaridade:** Comparação em tempo real entre uma imagem de consulta e o banco de dados.
* **Validação Visual:** Geração de gráficos de performance para garantir a confiabilidade das recomendações.



---

## 🛠️ Ferramentas e Tecnologias

Para a construção deste projeto, foram utilizadas as bibliotecas mais modernas do ecossistema de **Data Science**:

* **Linguagem:** `Python 3.x`
* **Frameworks de IA:** `TensorFlow` e `Keras` (Modelo ResNet50).
* **Processamento de Imagens:** `PIL (Pillow)` e `Matplotlib`.
* **Cálculo Vetorial:** `NumPy` e `Scikit-learn` (Distância Euclidiana).
* **Ambiente de Desenvolvimento:** `Google Colab` integrado ao `Google Drive`.

---

## 🔬 Detalhes Técnicos (O Diferencial)

O diferencial deste projeto está no rigor técnico aplicado em cada etapa:

### **1. Modelo ResNet50 e Extração de Vetores**
Utilizamos o modelo **ResNet50** pré-treinado. Removemos a camada final de classificação para extrair um vetor de **6.144 dimensões**. Isso significa que cada imagem é descrita por milhares de características únicas detectadas pela IA.

### **2. Validação de Performance (Acurácia)**
O sistema passou por uma fase de validação onde foram gerados gráficos de **Acurácia (Accuracy)** e **Perda (Loss)**. Isso garante que o motor de recomendação está calibrado e possui baixa taxa de erro.



### **3. Persistência de Dados**
Para garantir a escalabilidade, o conhecimento gerado foi exportado em arquivos `.p` (**Pickle**), permitindo que o sistema seja carregado instantaneamente sem a necessidade de reprocessar todas as imagens novamente.

---

## 🚀 Como Executar

1.  Clone este repositório.
2.  Abra o arquivo `.ipynb` no **Google Colab**.
3.  Monte o seu **Google Drive** para carregar os arquivos de índice.
4.  Suba uma imagem de teste para receber as recomendações.

---

## 🎓 Instituições e Parcerias

Este projeto é fruto do aprendizado obtido através da bolsa de estudos da:
* **DIO (Digital Innovation One)**
* **BairesDev**

---

> **Status do Projeto:** Concluído ✅

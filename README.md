# 🧪 SoluAI – Prevendo a Solubilidade de Compostos com Inteligência Artificial

Este projeto tem como objetivo prever a **constante de solubilidade (pKs)** de compostos químicos utilizando técnicas de **aprendizado de máquina**, como **Random Forest** e **Redes Neurais Profundas (DNN)**. o **autoral e experimental**.

---

## 📌 Introdução

A solubilidade é definida como a quantidade máxima de uma substância que pode ser dissolvida em uma certa quantidade de solvente. O processo de solubilização resulta de interações químicas entre a espécie que se almeja solubilizar e o solvente, sendo influenciado por parâmetros e propriedades químicas dentre as principais estão as forças intermoleculares, raio covalente, raio iônico, polaridade e temperatura. A solubilidade pode ser descrita pelo produto de solubilidade, o qual expressa a constante de equilíbrio da dissolução de um composto iônico em solução aquosa. (HARRIS, 2012)
	Conhecer a solubilidade é de grande importância para diversas indústrias, como farmacêutica, de cosméticos e química, pelo desenvolvimento de medicamentos, formulação de produtos à base de óleos essenciais, produção de fertilizantes, por exemplo. Martins et al. (2013) aborda um exemplo da importância do estudo sobre este tema em um incidente ocorrido no Brasil, em 2003, envolvendo medicamentos utilizados em exames de radioscopia e radiografia. Na ocasião, houve uma contaminação de um contraste a base de sulfato de bário com carbonato de bário, culminando no óbito de pelo menos 21 pessoas. Por ser praticamente insolúvel em água e soluções ácidas diluídas, o sulfato de bário ao ser aplicado em pacientes promove o destaque dos órgãos do sistema digestivo. Por sua vez, a presença de carbonato de bário, constatada posteriormente por análises químicas, é solúvel nessas condições e provoca a liberação de íons do metal, os quais apresentam riscos à vida humana devido a sua toxicidade. 
	A solubilidade é, portanto, um importante parâmetro que deve ser analisado frequentemente por meio de testes, exigindo gastos associados ao consumo de reagente e gerando resíduos químicos potencialmente prejudiciais ao meio ambiente. O uso de técnicas de Inteligência Artificial surge como uma alternativa para avaliar a solubilidade de compostos químicos a partir de propriedades químicas conhecidas, o que permite a redução dos custos e tempo das análises, além de mitigar impactos ambientais. Modelos preditivos com base em aprendizado de máquina, por exemplo, Random Forest e Redes Neurais Artificiais (ANN), conseguem identificar correlações entre as variáveis fornecidas e predizer uma saída. 
	Neste contexto, o trabalho tem como objetivo criar um modelo preditivo para avaliar a solubilidade de compostos químicos e determinar a constante de solubilidade (pKs). Para isso, será empregada uma abordagem que se baseia em técnicas de aprendizado de máquina, utilizando variáveis químicas extraídas de bases de dados confiáveis, como o "CRC Handbook of Chemistry and Physics" e o "Lange’s Handbook".

---

## 🔍 Objetivo

Criar modelos de IA capazes de prever a constante de solubilidade (**pKs**) de compostos iônicos com base em variáveis químicas como:

- Carga do íon
- Raio iônico
- Energia de ionização

---

## 🧠 Modelos Utilizados

### Random Forest
- 100 estimadores
- Critério: Erro quadrático médio (MSE)
- Resultados:  
  - MAE: 1.01  
  - MSE: 3.57

### Rede Neural Profunda (DNN)
- Arquitetura Feedforward (Keras + TensorFlow)
- Funções de ativação: ReLU
- Regularização com Dropout
- Otimizador: Adam | Épocas: 100
- Resultados:  
  - MAE: 1.01  
  - MSE: 2.36

---

## ⚙️ Tecnologias

- **Python**
- **Pandas**, **NumPy**, **Scikit-learn**
- **TensorFlow / Keras**
- **Matplotlib** e **Seaborn**

---

## 📈 Metodologia

1. **Coleta de Dados**  
   Fontes: *CRC Handbook* e *Lange’s Handbook*

2. **Pré-processamento**  
   - Codificação de variáveis categóricas (`LabelEncoder`, `OneHot`)
   - Normalização com `StandardScaler`
   - Imputação de dados ausentes

3. **Treinamento e Validação**  
   - Divisão treino/teste
   - Avaliação com MAE, MSE e curva de aprendizado
   - Visualizações: Gráfico pKs Real vs. Predito

---

## 📊 Resultados Visuais

- Curvas de aprendizado mostram boa convergência
- DNN teve desempenho superior ao Random Forest em MSE
- Redução expressiva de erro com normalização e ajuste de hiperparâmetros

---

## ✅ Conclusão

A aplicação de IA mostrou-se eficaz na previsão de pKs. A DNN otimizada superou a Random Forest, com maior capacidade de aprendizado e menor erro médio quadrático. Além dos ganhos científicos, o projeto propõe uma **solução econômica e sustentável**, reduzindo a necessidade de testes laboratoriais.

---


---

## 📚 Referências

- Harris, D. C. *Análise Química Quantitativa*, 8ª ed.  
- Gao et al. (1996). *Environmental Toxicology and Chemistry*  
- NobelPrize.org (2024, 2025)  
- Martins et al. (2013), Sena et al. (2000), Silva et al. (2004)  
- CRC Handbook / Lange's Handbook

---


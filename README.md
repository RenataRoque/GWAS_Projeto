
# Aplicação de métodos de aprendizado de máquina para identificação de regiões genômicas associadas a características agronômicas em arroz (*Oryza sativa*)

**Autores:** Renata Dourado Roque, Camila Ferreira Azevedo, Ana Carolina Campana Nascimento e Moyses Nascimento.

## Apresentação

A Associação Genômica Ampla (*Genome-Wide Association Study* – GWAS) é uma abordagem utilizada para identificar associações entre marcadores moleculares e características quantitativas, contribuindo para o melhoramento genético. Tradicionalmente, essas análises são conduzidas por meio de modelos lineares mistos (MLM). Entretanto, a complexidade genética de características agronômicas pode envolver relações não lineares e interações gênicas, aspectos que podem limitar o desempenho dos modelos tradicionais.

Nesse contexto, métodos de aprendizado de máquina (*Machine Learning* – ML) constituem alternativas para identificar marcadores relevantes e ampliar a investigação das regiões genômicas associadas a características agronômicas.

Este trabalho propõe a comparação e integração de diferentes métodos de aprendizado de máquina e GWAS, com o propósito de identificar e priorizar regiões genômicas associadas a características agronômicas em arroz (*Oryza sativa*).

## Objetivo

Comparar e integrar métodos de aprendizado de máquina e GWAS para identificar e priorizar regiões genômicas associadas a características agronômicas em arroz.

## Dados

Foram analisados 413 acessos de arroz (*Oryza sativa*), genotipados com 36.901 marcadores SNPs e fenotipados para quatro características agronômicas:

- Resistência à brusone (RB);
- Largura da folha bandeira (LFB);
- Flores por panícula (FP);
- Comprimento da panícula (CP).

Os dados são públicos e integram os projetos OryzaSNP e OMAP (AMMIRAJU et al., 2006; ZHAO et al., 2011), estando disponíveis no portal [Rice Diversity](https://ricediversity.org/data/).

## Metodologia

Foram avaliados sete métodos, distribuídos em duas categorias:

**Métodos de aprendizado de máquina (ML):**

- Árvore de Decisão (*Decision Tree*);
- Bagging;
- Boosting;
- Random Forest;
- *Multivariate Adaptive Regression Splines* (MARS).

**Métodos de GWAS:**

- *Mixed Linear Model* (MLM);
- FarmCPU.

A importância dos marcadores foi estimada por validação cruzada, enquanto a significância estatística foi avaliada por testes de permutação, permitindo a obtenção de valores-p empíricos com correção para múltiplos testes.

Posteriormente, as medidas de importância foram normalizadas e sintetizadas por regiões genômicas, possibilitando a integração das evidências fornecidas pelos diferentes métodos e a priorização de regiões associadas às características avaliadas.

## Principais resultados

Foram identificadas cinco regiões genômicas relevantes:

- Duas regiões associadas à resistência à brusone (RB);
- Uma região associada à largura da folha bandeira (LFB);
- Uma região associada a flores por panícula (FP);
- Uma região associada ao comprimento da panícula (CP).

As regiões associadas à resistência à brusone e à largura da folha bandeira foram identificadas por múltiplos métodos, indicando maior consistência entre as abordagens.

Os resultados demonstram que a integração de diferentes métodos permite priorizar regiões genômicas com evidências mais consistentes de associação. Além disso, regiões identificadas por métodos específicos podem refletir diferentes componentes genéticos das características avaliadas, ampliando o conjunto de regiões candidatas para validação funcional.

## Organização do repositório

O repositório está organizado nas seguintes pastas:

- **Scripts/**: códigos desenvolvidos em R e utilizados nas análises estatísticas e na aplicação dos métodos de aprendizado de máquina.
- **Data/**: informações sobre os dados utilizados na pesquisa, provenientes dos projetos OryzaSNP e OMAP. Os dados originais podem ser acessados no portal [Rice Diversity](https://ricediversity.org/data/).
- **Results/**: figuras, visualizações e resultados obtidos a partir das análises realizadas.

## Linguagem e ferramentas

As análises foram desenvolvidas utilizando a linguagem de programação R.

## Palavras-chave

GWAS; Aprendizado de máquina; Melhoramento genético; Testes de permutação; Efeitos não lineares.

## Referências

## Referências

AMMIRAJU, J. S. S. et al. The Oryza bacterial artificial chromosome library resource: construction and analysis of 12 deep-coverage large-insert BAC libraries that represent the 10 genome types of the genus Oryza. *Genome Research*, v. 16, n. 1, p. 140–147, jan. 2006.

BALLINI, E. et al. A genome-wide meta-analysis of rice blast resistance genes and quantitative trait loci provides new insights into partial and complete resistance. *Molecular Plant-Microbe Interactions*, v. 21, n. 7, p. 859–868, 2008.

MILLER, C. et al. A Review of Model Evaluation Metrics for Machine Learning in Genetics and Genomics. *Frontiers in Bioinformatics*, v. 4, p. 1457619, 2024.

ZHAO, K. et al. Genome-wide association mapping reveals a rich genetic architecture of complex traits in *Oryza sativa*. *Nature Communications*, v. 2, n. 1, p. 467, 2011.

---

**Trabalho apresentado na Reunião Anual da Sociedade Internacional de Biometria – RBras 2026.**

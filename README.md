# 📚 Análise do Saeb 2023 – Pernambuco

---

## 📝 Descrição do Projeto

Este projeto consiste na **análise dos resultados do Sistema de Avaliação da Educação Básica (Saeb) – 2023**, com foco no estado de **Pernambuco**.  

O objetivo principal é **avaliar a proficiência dos estudantes em Língua Portuguesa (LP) e Matemática (MT)** em diferentes etapas de ensino (5º ano, 9º ano e 3ª série do Ensino Médio) e **comparar o desempenho estadual com a média nacional**, a partir do conjunto de dados [`TS_UF_20250507.xlsx`](https://github.com/seu-usuario/nome-do-projeto/blob/main/TS_UF_20250507.xlsx).

---

## 📊 Estrutura dos Dados

| Coluna         | Descrição                                                      |
|----------------|----------------------------------------------------------------|
| CO_UF          | Código da Unidade da Federação                                  |
| NO_UF          | Nome da Unidade da Federação                                    |
| DEPENDENCIA_ADM| Dependência administrativa da escola (Estadual, Municipal...)  |
| LOCALIZACAO    | Localização da escola (Urbana ou Rural)                        |
| CAPITAL        | Se a escola está situada na capital ou no interior             |
| MEDIA_5_LP     | Proficiência média em Língua Portuguesa - 5º ano EF            |
| MEDIA_5_MT     | Proficiência média em Matemática - 5º ano EF                   |
| MEDIA_9_LP     | Proficiência média em Língua Portuguesa - 9º ano EF            |
| MEDIA_9_MT     | Proficiência média em Matemática - 9º ano EF                   |
| MEDIA_12_LP    | Proficiência média em Língua Portuguesa - 3ª série EM          |
| MEDIA_12_MT    | Proficiência média em Matemática - 3ª série EM                 |

---

## 🔧 Pré-processamento

- Leitura do arquivo Excel com o pandas (`pd.read_excel`).  
- Verificação das colunas disponíveis e filtragem dos dados para **Pernambuco**.  
- Cálculo das médias gerais por etapa de ensino para Pernambuco e para o Brasil.  
- Preparação de listas de médias para gráficos comparativos.

---

## 📈 Análises e Visualizações

### Proficiência Média por Etapa – Pernambuco
- **Língua Portuguesa**: aumento progressivo do 5º ano (~200) à 3ª série EM (~283).  
- **Matemática**: desempenho ligeiramente superior em quase todas as etapas (5º ano ~210, 3ª série EM ~285).  

### Comparativo Pernambuco x Brasil
- Pernambuco apresenta desempenho **próximo à média nacional**, ligeiramente inferior no 5º ano.  
- Diferença tende a **diminuir no Ensino Médio**, indicando melhora contínua.  

---

## 💡 Insights Principais

- O desempenho dos estudantes melhora conforme o avanço escolar, com **crescimento consistente do 5º ano ao Ensino Médio**.  
- A diferença em relação à média nacional diminui nas etapas finais, sugerindo **eficácia das políticas educacionais estaduais**.  
- Necessidade de **fortalecer aprendizagens nos anos iniciais** para garantir sucesso nas etapas seguintes.

---

## 🛠 Tecnologias e Bibliotecas

- Python 3  
- Pandas  
- Matplotlib  
- Jupyter Notebook  

---

## 🚀 Como Executar

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/nome-do-projeto.git

# Entrar no diretório
cd nome-do-projeto

# Instalar dependências
pip install -r requirements.txt

# Abrir o notebook
jupyter notebook

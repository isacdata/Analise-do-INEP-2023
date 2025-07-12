# 📘 Análise do ENEM 2023 – Desigualdade Educacional a partir dos Microdados do INEP

Este projeto realiza uma análise estatística exploratória e modelagem preditiva com base nos microdados do ENEM 2023, fornecidos pelo INEP. O foco está em investigar como fatores socioeconômicos influenciam o desempenho dos candidatos, evidenciando padrões de desigualdade educacional.

---

## 🎯 Objetivo

Entender **o quanto fatores como faixa etária, renda, escolaridade dos pais, etnia, tipo de escola e acesso à tecnologia** influenciam a nota final do ENEM.  
A partir disso, testar hipóteses sobre disparidades educacionais estruturais no Brasil.

---

## 📌 Hipóteses Investigadas ⭐

- ⭐ Qual faixa etária teve melhor desempenho no ENEM?
- ⭐ A renda familiar impacta significativamente a nota final?
- ⭐ O nível de escolaridade dos pais influencia o resultado?
- ⭐ Há diferença entre gêneros e entre grupos raciais?
- ⭐ Candidatos de escolas públicas têm desvantagem estatística?
- ⭐ Qual o perfil de quem tira mais de 750 pontos?
- ⭐ Quem fica abaixo de 500 pontos tem perfil comum?

---

## 📊 Dados Utilizados

- Fonte: Microdados do ENEM 2023  
- Origem: [gov.br/inep](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem)
- Tamanho bruto: ~500MB (não incluído neste repositório)
- Variáveis utilizadas:
  - Notas por área: `NU_NOTA_MT`, `NU_NOTA_LC`, `NU_NOTA_CH`, `NU_NOTA_CN`, `NU_NOTA_REDACAO`
  - Dados pessoais: `TP_SEXO`, `TP_COR_RACA`, `TP_ESCOLA`, `TP_FAIXA_ETARIA`
  - Questionário socioeconômico: `Q001–Q006` (renda, escolaridade, internet, computador)

---

## 🧪 Técnicas Utilizadas

- Estatística descritiva e análise exploratória com gráficos
- Testes de hipótese: ANOVA, t-test, chi²
- Regressão com `XGBoost` (target: nota final)
- Avaliação com R², MSE
- Pré-processamento com `OneHotEncoder` e `ColumnTransformer`

---

## 📁 Estrutura

```
analise-inep-2023/
├── notebooks/
│   ├── INEP23.ipynb            # Análise exploratória e estatística
│   └── ML Models.ipynb         # Modelagem preditiva
├── requirements.txt
└── README.md
```

---

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/seuusuario/analise-inep-2023.git
cd analise-inep-2023
```

2. Instale os pacotes:
```bash
pip install -r requirements.txt
```

3. Acesse os notebooks na pasta `/notebooks`

---

## 👤 Autor

Projeto desenvolvido por **Isac Vieira**, com interesse em análise educacional, estatística aplicada e ciência de dados com propósito social.

---

## 📄 Licença

Uso livre para fins educacionais. Dados utilizados seguem os termos públicos de acesso do INEP.


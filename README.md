<div align="center">

# 👋 Olá, eu sou o **Kalléu Ribeiro**
**Data & Analytics | Python | Visualização | Automação**

[![My Skills](https://skillicons.dev/icons?i=py,regex,pycharm,sqlite,git,github,powershell,windows,tableau,powerbi&theme=dark)](https://skillicons.dev)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kalleu%20Ribeiro-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kalleu-ribeiro/)
[![Gmail](https://img.shields.io/badge/Email-kalleu156%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kalleu156@gmail.com)

</div>

---

## 🔥 Projetos em Destaque

### 1) **Classificar Finanças IA** — extratos (conta + cartão) com regras YAML, Streamlit e Excel
Automatiza a classificação de extratos bancários **localmente**, sem banco de dados, gera **gráficos interativos** e exporta **Excel** pronto.

https://github.com/user-attachments/assets/3df37da1-a156-4834-b2b1-6c165acac57e

**Repositório:** <https://github.com/Kalloyer/Classificar_financas>

**Stack:** Python · Pandas · PyYAML · Typer (CLI) · Streamlit + Plotly · XlsxWriter

**Destaques**
- Ingestão de **múltiplas faturas** do cartão + extrato único da conta
- Unificação com `origem` (Conta/Cartão) e `fatura_ref` (mês/ano inferido do nome do arquivo)
- **Classificação automática** por regras regex em `configs/regras.yml` (sem sobrescrever categoria que já veio no cartão)
- Dashboard com filtros (**Período, Origem, Categoria**), gráficos **Total por categoria** e **Crédito × Débito**
- Exportação para Excel com planilhas **Lancamentos**, **Por_Categoria**, **Por_Origem** (formato **R$**)

**Como rodar (Windows 11)**
```powershell
git clone https://github.com/Kalloyer/Classificar_financas.git
cd Classificar_financas
python -m venv .venv
.\.venv\Scripts\Activate
pip install -r requisitos.txt

# Pipeline único (ingesta → unir → classificar → exportar)
python -m src.app pipeline --pasta-cartao "dados\brutos\cartao" --arquivo-conta "dados\brutos\corrente\extrato.csv"

# Dashboard
streamlit run src/app_streamlit.py
```
---

### 2) **Telecom Customer Churn Analysis** — SQL, Python, Power BI & Tableau
Análise e previsão de churn em telecom: exploração com SQL, modelagem em Python e dashboards em BI.

**Power BI Dashboard:**  
![Power BI Dashboard](https://github.com/user-attachments/assets/05a05c63-6240-4ca7-855f-39bfe235c740)

**Tableau Dashboard:**  
![Tableau Dashboard](https://github.com/user-attachments/assets/af27ed47-13a1-4fd2-95d0-f5f4065faab6)

**Repositório:** <https://github.com/Kalloyer/Analise_churn_telecom>

**Destaques**
- Exploração em **SQL**: churn rate, métodos de pagamento, contratos e serviços
- **Modelagem preditiva** em Python com identificação das variáveis mais impactantes
- **Dashboards** interativos em Power BI e Tableau

---

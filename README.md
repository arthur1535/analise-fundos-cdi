# 📊 Análise de Fundos de Investimento vs CDI

Sistema completo para análise de performance de fundos de investimento em comparação com o CDI, utilizando dados reais da CVM e Banco Central.

## 🎯 Funcionalidades

- **Download automático** de dados da CVM
- **Análise de performance** de fundos vs CDI
- **Gráficos comparativos** interativos
- **Dados reais** da Taxa Selic do Banco Central

## 📁 Estrutura do Projeto

```
testecdi/
├── cvm.py                    # Análise principal - dados CVM vs CDI
├── teste_cvm.py             # Testes de download da CVM
├── cdi                      # Análise detalhada de fundos com CDI real
└── README.md                # Este arquivo
```

## 🚀 Como Usar

### 1. Instalação das Dependências

```bash
pip install pandas numpy matplotlib requests openpyxl
```

### 2. Executar Análise Principal

```bash
python cvm.py
```



## 📈 Principais Análises

### 1. Análise Individual de Fundos (cvm.py)
- Busca por CNPJ específico na base da CVM
- Comparação com CDI usando dados reais da Selic
- Gráfico de performance acumulada
- Métricas de risco e rentabilidade

## 🔧 Configuração

### Alterar CNPJ do Fundo
No arquivo `cvm.py`, linha 62:
```python
cnpj_original = '29177012000178'  # Altere para o CNPJ desejado
```

### Alterar Período de Análise
No arquivo `cvm.py`, linhas 32-33:
```python
data_inicio = dt.date(2025, 3, 1)
data_fim = dt.date(2025, 6, 11)
```

## 🔍 Fontes de Dados

- **CVM**: Dados oficiais de cotas de fundos
- **Banco Central**: Taxa Selic diária real
- **Período**: Março a Junho de 2025

## 📋 Requisitos

- Python 3.7+
- Conexão com internet (para download da CVM)
- Arquivo CSV da Selic: `D:/user/taxa_selic_apurada.csv`


## 🎨 Gráficos Gerados

- `raptor_vs_cdi_real.png` - Comparativo principal
- `raptor_vs_cdi_final.png` - Versão formatada
- `raptor_vs_cdi_final.pdf` - Versão para apresentação

## 📝 Exemplo de Uso

```python
# Analisar fundo específico
cnpj = '29177012000178'
periodo = ('2025-03-01', '2025-06-11')

# Executar análise
python cvm.py

# Resultado esperado
# Rentabilidade do fundo: X.XX%
# CDI no período: X.XX%
# Gráfico salvo: raptor_vs_cdi_real.png
```

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para detalhes.

## 📞 Contato

- **Autor**: Arthur Pires Lopes
- **Email**: arthur.lopes1@ufu.br
- **LinkedIn**: Arthur Pires Lopes

---

⭐ **Se este projeto foi útil para você, considere dar uma estrela!** ⭐

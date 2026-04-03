# 🎰 Golden Reels — Slot Math Simulator

Simulador matemático de slot machine desenvolvido em Python para fins de estudo e portfólio na área de **Game Math Design** para o mercado de iGaming.

---

## 📊 Resultados

| Métrica | Valor |
|---|---|
| RTP Teórico calculado | 27.37% |
| RTP Simulado (10M rodadas) | 27.40% |
| Diferença | 0.03% ✅ |
| Hit Rate | 5.45% |
| Rodadas simuladas | 10.000.000 |

A diferença de apenas **0.03%** entre o RTP teórico e o simulado está dentro da margem exigida por laboratórios de certificação como GLI e eCOGRA (< 0.5%).

---

## 🎯 O que este projeto demonstra

- Cálculo matemático de RTP via combinatória
- Validação por simulação Monte Carlo (10 milhões de rodadas)
- Geração automática de Game Math Document profissional
- Exportação de relatório técnico em PDF e Excel
- Análise de Hit Rate e distribuição de prêmios
- Visualização da convergência do RTP (Lei dos Grandes Números)

---

## 🗂️ Estrutura do projeto

```
slot-simulator/
├── slot_simulator.py              # Código principal
├── Golden_Reels_Math_Document.xlsx  # Game Math Document gerado
├── Golden_Reels_Report.pdf          # Relatório técnico gerado
└── README.md
```

---

## ⚙️ Como funciona

### 1. Math Model
O jogo possui 5 rolos com 6 símbolos, cada um com pesos diferentes que determinam sua frequência de aparição:

| Símbolo | Peso | Prob. por rolo |
|---|---|---|
| Cereja | 30 | 30.0% |
| Limão | 25 | 25.0% |
| Laranja | 20 | 20.0% |
| Estrela | 15 | 15.0% |
| Diamante | 7 | 7.0% |
| Sete | 3 | 3.0% |

### 2. RTP Teórico
Calculado matematicamente via combinatória — soma de (probabilidade × pagamento) para todas as combinações possíveis.

### 3. Simulação Monte Carlo
Valida o RTP teórico rodando 10 milhões de rodadas e comparando o resultado real com o esperado. É o mesmo processo usado por laboratórios de certificação como GLI e eCOGRA.

### 4. Relatórios automáticos
O projeto gera automaticamente:
- **Excel** com 4 abas: resumo, probabilidades, RTP detalhado e histórico
- **PDF** com tabelas, gráficos e conclusão de validação

---

## 🚀 Como rodar

### Instalar dependências
```bash
pip install numpy pandas matplotlib openpyxl reportlab
```

### Executar
```bash
python slot_simulator.py
```

Os arquivos Excel e PDF serão gerados automaticamente na pasta `output/`.

---

## 📚 Conceitos aplicados

- **RTP (Return to Player)** — percentual de retorno ao jogador
- **Hit Rate** — frequência de rodadas vencedoras
- **Volatilidade** — distribuição dos prêmios ao longo do tempo
- **Monte Carlo** — validação estatística por simulação massiva
- **Lei dos Grandes Números** — convergência do RTP com o aumento de rodadas
- **Game Math Document** — documento técnico padrão da indústria de iGaming

---

## 🛠️ Tecnologias

![Python](https://img.shields.io/badge/Python-3.12-blue)
![NumPy](https://img.shields.io/badge/NumPy-latest-blue)
![Pandas](https://img.shields.io/badge/Pandas-latest-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-latest-blue)

---

## 👨‍💻 Autor

**Gleuson Paiva**
Desenvolvedor Python | Automação com IA | Game Math Designer em formação

[![GitHub](https://img.shields.io/badge/GitHub-GleusonPaiva-black)](https://github.com/GleusonPaiva)

---

## 📌 Próximos projetos

- [ ] Projeto 2 — Slot com 10 linhas de pagamento e análise de volatilidade
- [ ] Projeto 3 — Modo bônus com free spins e multiplicadores
- [ ] Projeto 4 — Comparador de math models com relatório automático via IA
- [ ] Projeto 5 — Jogo completo com interface visual

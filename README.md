
# 3 GHz 90° Hybrid Coupler

Projeto de um **acoplador híbrido de 90°** operando em **3 GHz**, com **fator de acoplamento de –25 dB**, desenvolvido e otimizado através de simulações eletromagnéticas no **Ansys HFSS**.  
O dispositivo foi **fabricado em microfita** sobre substrato **Rogers 5880** e caracterizado experimentalmente em laboratório para validação dos parâmetros S.

## 📡 Visão Geral

O objetivo do projeto foi projetar, simular, fabricar e validar um **acoplador direcional de microfita de três estágios**, garantindo alto isolamento e baixa perda de retorno na faixa de 3 GHz.  
O projeto segue o fluxo completo de **simulação–para–hardware**, abrangendo modelagem teórica, otimização de desempenho e comparação entre resultados simulados e medidos.

## ⚙️ Especificações do Projeto

| Parâmetro | Valor / Descrição |
|------------|-------------------|
| Frequência central | 3 GHz |
| Tipo de acoplador | Híbrido 90° |
| Fator de acoplamento | –25 dB |
| Substrato | Rogers 5880 (εr = 2.2, h = 0.787 mm) |
| Tecnologia | Microfita |
| Ferramenta de simulação | Ansys HFSS |
| Portas | 4 (entrada, saída, acoplada e isolada) |

## 🧠 Metodologia

1. **Modelagem teórica:** Aplicação da teoria de linhas de transmissão em microfita para definir impedâncias e larguras das trilhas.  
2. **Simulação EM (HFSS):** Modelagem tridimensional do acoplador e ajuste paramétrico para atingir o fator de acoplamento desejado.  
3. **Otimização:** Ajuste fino de dimensões para melhorar o isolamento e a correspondência de impedâncias.  
4. **Fabricação:** Produção da placa em substrato **Rogers 5880** utilizando processo de fotolitografia.  
5. **Medições:** Comparação entre **S-parâmetros simulados e medidos**, validando a precisão do modelo.

## 📈 Resultados Obtidos

- Excelente concordância entre resultados simulados e experimentais.  
- Isolamento superior a 25 dB na faixa de operação.  
- Boa correspondência de impedâncias em todas as portas (S11 < –20 dB).  
- Fase de 90° entre portas de saída validada experimentalmente.  

### Exemplo de resultados (S-parâmetros)

| Parâmetro | Valor Simulado | Valor Medido |
|------------|----------------|---------------|
| S11 (Retorno) | –22.5 dB | –20.8 dB |
| S21 (Transmissão) | –3.1 dB | –3.2 dB |
| S31 (Acoplado) | –25.0 dB | –25.4 dB |
| S41 (Isolamento) | –28.5 dB | –27.9 dB |

## 🧩 Estrutura do Projeto

```
90HybridCoupler/
│
├── simulation/             # Arquivos e modelos HFSS (.aedt)
├── fabrication/            # Layouts de fabricação e fotos do protótipo
├── measurements/           # Resultados experimentais e S-parâmetros medidos
├── docs/                   # Relatórios e documentação técnica
└── README.md               # Este arquivo
```

## 🔬 Conceitos Envolvidos

- Teoria de linhas de transmissão em microfita.  
- Acoplamento direcional e defasagem de 90°.  
- Casamento de impedâncias e isolamento entre portas.  
- Simulações eletromagnéticas 3D no HFSS.  
- Validação experimental via medições de S-parâmetros.  

## 🚀 Próximos Passos

- Análise de sensibilidade para tolerâncias de fabricação.  
- Extensão do projeto para frequências mais altas (5–10 GHz).  
- Implementação de varredura de banda para avaliar desempenho fora da faixa central.  

## 📄 Licença

Este projeto é de código aberto sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---

Autor: [Gabriel Bozelli](https://github.com/gbozelli)  
Engenharia de Telecomunicações — UNESP  
Bolsista FAPESP | Projeto de Dispositivos RF e Simulação Eletromagnética

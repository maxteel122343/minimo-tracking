# Documentação do Projeto: Rastreamento Multimodal Mínimo para Robótica e Saúde Assistida

**Versão:** Fase 7 + Mapeamento  
**Data:** 27 de novembro de 2026  
**Objetivo:** Documentar o processo SCAMPER, descobertas, caminhos tecnológicos e MVPs para rastreamento não invasivo / de baixo hardware de dados humanos (gestos, movimento, biomarcadores) com uso dual em treino de robótica e saúde assistida por IA.

## Arquivos deste conjunto

| Arquivo | Conteúdo |
|---------|----------|
| `01-visao-geral.md` | Este arquivo – índice e visão geral |
| `02-scamper-fases.md` | Resumo consolidado das Fases 1 a 7 do SCAMPER |
| `03-descobertas-tecnologicas.md` | Inovações, tecnologias-chave e fundamentação |
| `04-mapeamento-4-eixos.md` | Mapeamento nas 4 direções (inovação, comercial, artigos, MVP) |
| `05-mvp-roadmap.md` | Roadmap de produto e MVPs concretos |
| `06-referencias-e-pilares.md` | Pilares conectados, referências e notas de continuidade |

## Visão Geral do Projeto

O trabalho explora caminhos **não invasivos e de mínimo hardware** para capturar dados ricos de movimento humano e biomarcadores, com três pilares interconectados:

1. **Dados para Robótica e IA** – demonstrações humanas, gestos, manipulação, toque, face.
2. **Marcadores Biológicos** – HR, RR, pH, redox, íons, temperatura, etc., com foco em categorias e proxies (não cobertura total dos milhares de marcadores).
3. **Vibecode Hardware e Automação** – ESP32, leitores de frequência, tintas comestíveis, sensores passivos.

**Tecnologias integradoras principais:**
- Smartphone como hub universal (câmera, IMU, toque, MediaPipe/ARKit, rPPG).
- Sensores passivos de frequência (LC / SRR / exceptional points) multiplexados.
- Eletrônica e tintas comestíveis / ingeríveis.

**Princípio guia:** maximizar dados e marcadores com o mínimo de hardware e atrito para o usuário, priorizando implementação rápida de MVP.

## Como usar esta documentação

- Use este índice como ponto de entrada.
- Consulte `04-mapeamento-4-eixos.md` para decisões estratégicas.
- Use `05-mvp-roadmap.md` para planejamento de implementação.
- Atualize os arquivos conforme novas fases ou validações.

---

*Documentação gerada para continuidade do processo SCAMPER aplicado a sensores, biomarcadores e dados de robótica.*

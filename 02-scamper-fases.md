# SCAMPER – Resumo Consolidado das Fases 1 a 7

Processo iterativo de exploração e refinamento. Cada fase aproximou de protótipos reais e eliminou equívocos.

## Fases iniciais (1–3)
- Mapeamento de ideias originais (escrita, gestos no celular, olhos, toque, mastigação, face, linguagem de sinais, animais, cordas vocais, órgãos internos, etc.).
- Aplicação sistemática do SCAMPER com foco em sensores.
- Integração dos 3 pilares: dados de robótica, marcadores biológicos e vibecode hardware.
- Prioridade em MVP rápido e caminhos do mais acessível ao mais avançado.

## Fase 4
- Maximizar marcadores com mínimo ou zero hardware extra.
- Celular como base principal (rPPG, IMU, MediaPipe).
- Vibecode para descobrir hardware relevante de baixo custo.
- Diversidade de formas de rastreamento com boa experiência do usuário.

## Fase 5
- Destaque para **tinta comestível + frequência** como tecnologias integradoras.
- Correção de escopo: existem centenas de milhares de possíveis marcadores; estratégia é categorias + proxies + multiplexação.
- Caminhos não invasivos e de mínimo hardware como achados centrais.

## Fase 6
- Integração de pesquisas recentes (2024–2026):
  - Multiplexação passiva (temperatura + íons + pH + glicose etc.).
  - Eletrônica comestível avançada (LC/SRR em açúcar, massa, gelatina).
  - Phone2Act e sistemas de captura egocêntrica via smartphone.
- Arquitetura em camadas consolidada.
- Eliminação de expectativas irreais de cobertura total de marcadores.

## Fase 7
- Especificação de protótipo mínimo.
- Substituição por sensores passivos + celular como hub.
- Combinação clara: app celular + leitor ESP32 opcional + sensor LC/SRR.
- Adaptação de projetos open-source de medidores de frequência.
- MVP em camadas com tempos estimados.

## Evolução principal do SCAMPER

| Letra | Descoberta consolidada |
|-------|------------------------|
| **S** | Substituir múltiplos sensores ativos por passivos de frequência + celular |
| **C** | Combinar celular multimodal + frequência passiva + vibecode |
| **A** | Adaptar leitores ESP32 open-source e tintas comestíveis existentes |
| **M** | Modificar para começar com 1–2 marcadores bem definidos e expandir |
| **P** | Usar dual-use (saúde pessoal + dados de robótica) |
| **E** | Eliminar bateria no sensor, múltiplos dispositivos e promessas de cobertura total |
| **R** | Reorganizar em camadas: celular → ESP32 → comestível |

## Princípios que se mantiveram
- Mínimo hardware e atrito.
- Consentimento e valor imediato para o usuário.
- Dados ricos para robótica em paralelo à saúde.
- Iteração rápida via vibecode.
- Fundamentação em pesquisas reais.

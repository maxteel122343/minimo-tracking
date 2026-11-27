# Pilares, Referências e Notas de Continuidade

## Os Três Pilares Conectados

1. **Dados para Robótica e IA**
   - Demonstrações humanas de manipulação, gestos, toque, face.
   - Captura via celular (Phone2Act, MediaPipe, egocêntrico).
   - Formatos abertos (estilo LeRobot) para treino de políticas VLA.

2. **Marcadores Biológicos**
   - Estratégia: categorias + proxies + multiplexação (não cobertura total).
   - Prioritários: vitais (HR, RR), eletrolíticos/metabólicos simples, pH, redox, temperatura, strain.
   - Fontes: celular (rPPG/IMU) + sensores de frequência passivos/comestíveis.

3. **Vibecode Hardware e Automação**
   - ESP32 e circuitos abertos de leitura de frequência.
   - Tintas e elementos comestíveis fabricáveis.
   - Acelera iteração e expansão da capacidade de captura.

**Conexão:** o vibecode permite criar hardware mínimo que expande tanto os dados de robótica quanto os marcadores biológicos capturáveis com baixo atrito.

## Referências-Chave (resumo)

### Sensores de Frequência e Multiplexação
- Science Advances (2025): multiplexed wireless sensing system (high-order exceptional points).
- ACS Applied Materials & Interfaces (2025): Flexible Passive Wireless Sensing Platform with Frequency Mapping.

### Eletrônica Comestível
- Advanced Engineering Materials / Advanced Materials Technologies (2024–2026): edible LC, SRR, solenoids, isotropic cubes.
- Trabalhos de tintas sprayáveis condutivas (carvão + goma/gelatina).
- arXiv: Edible Resonators.

### Ingestíveis
- GISMO (imec) e revisões de cápsulas para redox, pH, temperatura (Device 2025 e first-in-human).

### Dados de Robótica via Smartphone
- Phone2Act: smartphone como controlador 6-DoF e coleta para VLA.
- MobileEgo Anywhere, Surgical Intelligence Labs, egocentric hand tracking papers/repos (2025–2026).

### Bases de Biomarcadores
- MarkerDB (~34.500 catalogados).
- HMDB e espaço metabólico amplo (estratégia de proxies necessária).

## Notas para Continuidade

- Atualizar este conjunto de arquivos a cada nova fase SCAMPER ou validação experimental.
- Próximos passos possíveis:
  - Detalhamento técnico do fluxo de dados e formato de exportação.
  - Esquema de sensor LC comestível simples.
  - Lista expandida de artigos com links e DOIs.
  - Protótipo de firmware ESP32.
  - Testes de bancada planejados.
- Manter o princípio de mínimo hardware e valor dual-use.
- Registrar equívocos eliminados e decisões de escopo.

## Estrutura de Arquivos Recomendada para Expansão
```
docs/
├── 01-visao-geral.md
├── 02-scamper-fases.md
├── 03-descobertas-tecnologicas.md
├── 04-mapeamento-4-eixos.md
├── 05-mvp-roadmap.md
├── 06-referencias-e-pilares.md
├── experimentos/          (futuro)
├── referencias/           (futuro – PDFs ou links)
└── prototipos/            (futuro – código e esquemas)
```

---

*Documentação de consulta e continuidade – processo SCAMPER aplicado a sensores passivos, eletrônica comestível, smartphone como hub e dados dual-use para robótica e saúde.*

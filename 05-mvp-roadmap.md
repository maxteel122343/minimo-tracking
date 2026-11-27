# Roadmap de Produto e MVPs

## Visão do Produto
Aplicativo + sensores opcionais mínimos que capturam dados multimodais (gestos, toque, face, vitais, marcadores de frequência) para:
- Treino de modelos de robótica (demonstrações humanas).
- Saúde assistida pessoal em tempo real com IA.

## Camadas de MVP

### MVP 0 – Celular Puro (mais rápido)
- **Hardware:** apenas smartphone.
- **Funcionalidades:**
  - Captura de mãos e gestos (MediaPipe / ARKit).
  - Face, expressões e olhos.
  - Estimativa de HR e RR (rPPG).
  - Movimento do dispositivo (IMU) e toque.
- **Valor:** biofeedback imediato + geração de dados de robótica.
- **Tempo estimado:** dias.
- **Exportação:** vídeo + timestamps + vetores de pose.

### MVP 1 – Celular + Leitor de Frequência
- **Hardware:** smartphone + ESP32 (vibecode) com circuito de interrogação LC/frequência.
- **Adicional:** leitura de 1–2 sensores passivos (patch ou objeto).
- **Marcadores extras:** temperatura, pH, strain ou similar.
- **Comunicação:** Bluetooth com o app.
- **Tempo estimado:** 1–2 semanas após MVP 0.
- **Base técnica:** projetos open-source de medidores LC para ESP32.

### MVP 2 – Sensor Comestível / Ingerível
- **Hardware:** MVP 1 + elemento LC/SRR comestível (ouro, carvão, gelatina, amido/açúcar).
- **Formas:** cápsula, chiclete, revestimento.
- **Marcadores:** pH, temperatura, redox aproximado no GI ou oral.
- **Tempo estimado:** semanas adicionais.
- **Nota:** usar materiais e formulações já demonstradas em papers.

### MVP 3 – Pipeline Dual-Use Completo
- Sincronização robusta de todos os streams.
- Exportação em formato útil para treino (compatível ou convertível para estilo LeRobot: Parquet + vídeo).
- Dashboard de saúde pessoal com IA.
- Opções de consentimento e compartilhamento de dados.

## Fluxo de Dados Sugerido
1. Captura no celular (e no ESP32 se presente).
2. Sincronização por timestamps.
3. Armazenamento local ou cloud (com consentimento).
4. Exportação para:
   - Formato de dataset de robótica.
   - Visualização / feedback pessoal.

## Prioridade de Implementação
1. MVP 0 (validar experiência e captura).
2. MVP 1 (adicionar leitor de frequência e um sensor passivo simples).
3. MVP 2 (sensor comestível como extensão).
4. Refinamento do pipeline e valor dual-use.

## Componentes de Vibecode Recomendados
- ESP32 + circuito de medidor LC / interrogador de frequência.
- Templates de firmware para leitura e envio via Bluetooth.
- Prototipagem rápida de elementos ressonantes e tintas.

## Riscos e Mitigações
- **Precisão de marcadores:** começar com poucos e bem caracterizados; calibrar incrementalmente.
- **Experiência do usuário:** valor imediato de biofeedback para incentivar uso.
- **Regulatório:** MVP inicial não clínico; sensores externos ou comestíveis simples.
- **Privacidade:** consentimento claro e controle dos dados pelo usuário.

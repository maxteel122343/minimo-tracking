# Descobertas Tecnológicas e Fundamentação

## 1. Sensores Passivos de Frequência Multiplexados
- **Princípio:** deslocamento de frequência de ressonância (LC, SRR ou high-order exceptional points) codifica múltiplos parâmetros.
- **Capacidades demonstradas:** temperatura, umidade, Na⁺, K⁺, pH, glicose, amônio, proximidade, strain.
- **Vantagens:** sem bateria, baixo custo, leitura externa, stretchable ou comestível.
- **Referências principais:** Science Advances (2025) – multiplexed wireless sensing; ACS Applied Materials & Interfaces (2025) – frequency mapping.

## 2. Eletrônica e Tintas Comestíveis
- LC e SRR totalmente comestíveis:
  - Ouro comestível em espaguete/massa.
  - Cubos de açúcar/isomaltulose + papel de amido com SRR.
  - Gelatina + metal leaf.
- Tintas sprayáveis: carvão ativado + goma/gelatina (gauge factor 19–92 para strain).
- Uso em GI, oral, ou como revestimento degradável.
- **Referências:** Advanced Engineering Materials, Advanced Materials Technologies, arXiv Edible Resonators, revisões de edible electronics (2024–2026).

## 3. Smartphone como Hub Universal
- **Sensores nativos:** câmera (rPPG, face, mãos via MediaPipe/ARKit), IMU, microfone, toque, barômetro.
- **Capacidades:** HR/RR estimados, pose de mãos 21 pontos, gestos, expressões, movimento.
- **Dados de robótica:** Phone2Act (smartphone como controlador 6-DoF), MobileEgo, Surgical Intelligence Labs – exportação para formatos de treino (estilo LeRobot).
- Zero hardware extra no MVP inicial.

## 4. Cápsulas e Sensores Ingeríveis
- GISMO (imec) e similares: redox/ORP + pH + temperatura ao longo do trato GI em humanos.
- Versões passivas de frequência reduzem complexidade em relação a cápsulas ativas.

## 5. Vibecode e Hardware Aberto
- ESP32 + circuitos simples de interrogação de frequência (projetos open-source de medidores LC e analisadores).
- Permite iteração rápida de leitores e conexão com sensores passivos.
- Templates facilitam expansão por terceiros.

## Categorias de Marcadores Prioritárias (estratégia de proxies)
- **Vitais e movimento:** HR, RR, SpO₂ estimado, pose, toque (celular).
- **Eletrolíticos / metabólicos de superfície:** Na⁺, K⁺, pH, lactato, glicose em suor (sensores passivos).
- **Internos GI:** pH, redox, temperatura (comestíveis/ingeríveis).
- **Movimento fino:** mãos, gestos, pressão de toque (robótica).

**Nota importante:** o espaço de marcadores é enorme (MarkerDB ~34k catalogados; espaço metabólico muito maior). A abordagem é por categorias + multiplexação + proxies, não cobertura exaustiva.

## Arquitetura em Camadas
1. Camada 0: só celular.
2. Camada 1: celular + ESP32 leitor de frequência.
3. Camada 2: + sensor comestível/ingerível LC/SRR.
4. Camada 3: multiplexação avançada + IA em tempo real.

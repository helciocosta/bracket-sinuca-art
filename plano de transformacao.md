🎱 Plano de Transformação: Ranking de Sinuca ART

Este documento organiza as modificações para adaptar o sistema "Bracket" para um ranking focado exclusivamente em duas modalidades competitivas.

1. Modalidades Oficiais do Ranking

[ ] Sinuca - Regra Brasileira:

Uso da bola 1 (vermelha) e as coloridas.

Regras de "castigo" e sequência de bolas.

Pontuação baseada no valor nominal das bolas.

[ ] Snooker - Regra Six Reds:

Variante com 6 bolas vermelhas.

Regras internacionais da WPBSA adaptadas para torneios rápidos.

Pontuação por cores: Vermelha (1), Amarela (2), Verde (3), Marrom (4), Azul (5), Rosa (6) e Preta (7).

2. Regras de Pontuação e Ranking (Backend)

As alterações serão feitas na lógica de processamento de resultados:

Ranking Contínuo: Implementar um sistema de pontos acumulados por temporada (Season).

Critérios de Desempate:

Saldo de partidas (frames).

Confronto direto.

Média de pontos por partida.

Bônus Especial: Pontuação extra para quem atingir a "Tacada Máxima" (Clearance) em cada regra.

3. Identidade Visual e UI (Frontend)

[ ] Tematização: Substituir o azul padrão do Bracket pelo Verde Bilhar (#2d5a27) e detalhes em Dourado.

[ ] Tradução e Termos:

"Tournament" ➔ "Torneio / Etapa"

"Match" ➔ "Confronto"

"Sets/Frames" ➔ "Partidas / Frames"

[ ] Dashboard de Ranking: Criar uma página dedicada para exibir o Top 10 de cada uma das duas modalidades.

4. Próximos Passos Técnicos

Localizar Modelos: Identificar onde o Bracket armazena os tipos de torneio para injetar "Regra Brasileira" e "Six Reds".

Ajuste de Pontos: Modificar a API para aceitar resultados parciais de frames.

Logotipo: Inserir a marca "Sinuca ART" no cabeçalho.

Status Atual: Ambiente de desenvolvimento configurado (Porta 5173/8400). Próxima tarefa: Alterações visuais iniciais.

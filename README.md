# Painel TSE — 2º turno 2026

Painel web (um único `index.html`, sem build) para acompanhar a apuração do 2º turno das Eleições 2026 com os dados públicos de divulgação do TSE (`resultados.tse.jus.br`).

- Placar nacional para Presidente, com seções totalizadas, comparecimento, abstenção, brancos e nulos
- Mapa-grade dos estados colorido pelo candidato que lidera (intensidade = vantagem)
- Detalhe por estado e tabela ordenável por UF
- Alterna entre Presidente e Governador (estados com 2º turno)
- Atualização automática (30 s, 1 min, 2 min ou manual)

## Como abrir

Os dados são lidos direto pelo navegador, então basta abrir o `index.html`:

- **GitHub Pages:** Settings → Pages → Deploy from branch → `main` / root. O painel fica em `https://<usuario>.github.io/painel_tse/`.
- **Local:** baixe o arquivo e abra no navegador.

O painel usa o código de eleição `6258` (2º turno de 2026) e lê os arquivos `/oficial/ele2026/6258/dados/<uf>/<uf>-c<cargo>-e006258-u.json`. Para usar outro código, informe na própria página ou pela URL: `index.html?ele=6258`.

`index.html?demo` mostra dados simulados, apenas para testar o visual.

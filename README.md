# Acompanhamento das PRs

Página que lê as planilhas de forecast (PRs) e as consolidadas (Prévia PréCierre, PréCierre, Prévia Cierre, Cierre) **no próprio navegador**.

- Nenhum dado fica neste repositório nem é enviado para fora: os números ficam só no navegador de quem usa.
- Opcional: senha em Ajustes, que guarda os dados criptografados (AES-GCM).
- Arquivo único (`index.html`), com a biblioteca SheetJS embutida.

## Tela inicial e publicação automática

- Dois botões (Rateio Horizontais / Acompanhamento PRs), cada um com a sua senha. Cada área vai cifrada (AES-GCM, chave por PBKDF2) e a senha não fica no arquivo.
- Quem tem uma chave do GitHub guardada no navegador publica sozinho as mudanças: os arquivos `rateio-dados.enc` e `prs-dados.enc` também vão cifrados com a senha da área. Quem abre o link recebe a última versão.

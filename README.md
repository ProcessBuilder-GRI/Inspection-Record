# GRI Qualidade - Controle de Inspeções

Aplicativo web estático para GitHub Pages. A versão inicial funciona no navegador e salva dados em `localStorage`.

## Publicação no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie `index.html`, `styles.css` e `app.js` para a raiz.
3. Abra **Settings > Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**, branch `main` e pasta `/root`.
5. Abra o endereço apresentado pelo GitHub.

## Primeiro acesso
- Matrícula: `1774`
- Perfil: `ADM`

## Importante para produção
GitHub Pages hospeda somente os arquivos estáticos. Esta versão usa armazenamento local, portanto cada dispositivo possui dados próprios. O controle de matrícula no navegador não é autenticação segura.

Para uso multiusuário real, substitua o módulo `load/save` por um backend, como Supabase, Firebase ou uma API corporativa, e aplique autenticação, banco central, trilha de auditoria e regras de acesso no servidor. Não coloque chaves administrativas ou segredos no JavaScript público.

## Funcionalidades
- Perfis inspetor, produção e ADM.
- Cadastro de usuários restrito ao ADM.
- Solicitação, início e fim de inspeções e reinspeções ilimitadas.
- Pendências marcáveis, reparo e nova solicitação.
- Soma de tempos de inspeção e espera.
- Ocorrências e justificativas.
- Indicadores e exportação em PDF com seletor de arquivo quando suportado.

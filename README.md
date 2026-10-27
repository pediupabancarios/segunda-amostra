# Segunda Amostra — Hemocentro de João Pessoa

PWA (arquivo único `index.html`) para solicitação e acompanhamento de segunda amostra
de doadores: pedido de exames, registro de resultados, acompanhamento do caso
(teleconsulta, confirmatórios, encaminhamento) e relatórios (PDF/CSV).

- **Backend:** Supabase `ohuaoncwgioawgptyqgz`, tabelas `sa_casos` e `sa_usuarios`.
- **Login:** nome de usuário + senha (Supabase Auth; conta criada pela RPC `sa_cadastrar` com e-mail sintético `<usuario>@sa.hemocentro.invalid`). Só entra quem estiver em `sa_usuarios`
  com `ativo = true` (RLS). Administradores liberam acesso na tela **Usuários**.
- **Deploy:** GitHub Pages (branch `main`, raiz).

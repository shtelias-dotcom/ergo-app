# CESAROLI ERGO — Aplicativo de Avaliação Ergonômica

Aplicativo web (PWA) de avaliação ergonômica conforme **REBA**, **RULA**, **NR-17** e **ISO 11226**.

**Desenvolvido por:** SHT Serviços e Com. Equip. Ind. Lab. Med. e Seg. Ltda.
**Responsável técnico:** Elias Fontes Cancio — CREA-SP 5071087346
**Versão:** 1.0.0-beta
**Licença BETA:** válida até 10/02/2027

---

## 🚀 Como publicar no GitHub Pages (grátis — 10 minutos)

### Pré-requisitos (conta gratuita)
1. Crie uma conta em [github.com](https://github.com) (se ainda não tiver)
2. Confirme seu e-mail

### Passo a passo

**1. Criar o repositório**
- Clique em **New repository** (botão verde)
- Nome do repositório: `ergo-app`
- Marque como **Public**
- Marque **Add a README file**
- Clique em **Create repository**

**2. Subir os arquivos**
- Na página do repositório, clique em **Add file → Upload files**
- Arraste os arquivos do app: `index.html`, `app.html`, `manifest.json`, `README.md`
- Em **Commit changes**, escreva: `Primeira versão do app CESAROLI ERGO`
- Clique em **Commit changes**

**3. Ativar GitHub Pages**
- Vá em **Settings** (aba no topo)
- No menu lateral, clique em **Pages**
- Em **Source**, selecione **Deploy from a branch**
- Em **Branch**, selecione **main** e pasta **/ (root)**
- Clique em **Save**
- Aguarde 1-2 minutos

**4. Pronto!**
- Seu app estará disponível em:
  `https://SEU_USUARIO.github.io/ergo-app/`
- Compartilhe esse link com a equipe

---

## 👤 Credenciais de acesso (fase beta)

| Usuário | E-mail | Senha |
|---|---|---|
| Admin | `elias@sht.com.br` | `SHT@2026` |
| Eduardo | `eduardo@sht.com.br` | `Ergo@2026` |
| Leandro | `leandro@sht.com.br` | `Ergo@2026` |
| Demonstração | `demo@sht.com.br` | `demo123` |

**IMPORTANTE:** As senhas estão no código. Para a fase beta é aceitável — mas antes de vender, migre para backend (Supabase) com senha criptografada.

---

## 📱 Instalar como app no celular

**Android (Chrome):**
1. Abra o link do app no Chrome
2. Toque nos 3 pontinhos (⋮) no canto superior direito
3. Toque em **Instalar app** ou **Adicionar à tela inicial**
4. O ícone aparece como aplicativo nativo

**iPhone (Safari):**
1. Abra o link no Safari
2. Toque no botão **Compartilhar** (quadrado com seta para cima)
3. Role e toque em **Adicionar à Tela de Início**
4. O ícone aparece como aplicativo nativo

---

## ✏️ Como adicionar novos usuários

Edite o arquivo `index.html`, localize o bloco `const USERS = {` (linha ~235) e adicione:

```javascript
const USERS = {
  'elias@sht.com.br':   { pw: 'SHT@2026',  name: 'Elias Fontes Cancio', role: 'admin',  crea: 'CREA-SP 5071087346' },
  'novo.usuario@sht.com.br': { pw: 'SenhaNova@2026', name: 'Nome Completo', role: 'avaliador' },
  // ...
};
```

Salve, envie para o GitHub (Upload files → Replace) e em 2 minutos a atualização está no ar.

---

## 📂 Estrutura dos arquivos

```
ergo-app/
├── index.html      → Tela de login
├── app.html        → Aplicação principal (avaliação REBA/RULA)
├── manifest.json   → Configuração PWA (ícone, cor, nome)
└── README.md       → Este arquivo
```

---

## 🛣️ Próximas evoluções (roadmap comercial)

**Fase 1 — Beta interna (ATUAL)**
- ✅ Login local para equipe SHT
- ✅ Avaliação REBA/RULA Passo 2
- ✅ Score em tempo real
- ✅ PWA instalável

**Fase 2 — Produto comercial**
- [ ] Passos 1, 3 e 4 do fluxo completo (postura, pescoço, pernas)
- [ ] Geração de laudo PDF assinado digitalmente
- [ ] Backend Supabase (autenticação profissional)
- [ ] Dashboard administrativo (controle de licenças)
- [ ] Pagamento recorrente (Stripe)

**Fase 3 — App nas lojas**
- [ ] Conversão para Flutter (código único Android/iOS)
- [ ] Google Play Store
- [ ] Apple App Store

---

**Contato:** sht.elias@gmail.com
**Endereço:** Av. Ataliba Pontes, 210 - Pq. Paineiras, Sorocaba/SP - CEP 18078-613

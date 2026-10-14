# 🌟 Centralizador de Links & Bio Profissional de Alto Padrão

Uma alternativa de alto padrão, elegante e responsiva ao Linktree, criada especificamente para **profissionais liberais** (psicólogas, advogadas, médicas, consultoras e executivas).

Desenvolvido com foco em **mobile-first**, tipografia editorial refinada (*Cormorant Garamond* & *Plus Jakarta Sans*), micro-interações táteis e **seletor global de tema claro/noturno com alto contraste**.

---

## 🚀 Como Fazer Deploy na Vercel

O projeto já está 100% configurado com `vercel.json` e scripts otimizados para deploy instantâneo na Vercel sem nenhum erro.

### Passo 1: Subir para o seu GitHub
Abra o terminal no diretório do projeto e execute:

```bash
# 1. Inicialize o repositório git (caso ainda não esteja inicializado)
git init

# 2. Adicione todos os arquivos
git add .

# 3. Crie o primeiro commit
git commit -m "feat: Centralizador de Links de Alto Padrão"

# 4. Conecte com o seu repositório no GitHub (substitua pela sua URL)
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git

# 5. Envie para o GitHub
git push -u origin main
```

### Passo 2: Importar na Vercel
1. Acesse [vercel.com](https://vercel.com) e faça login.
2. Clique em **"Add New..."** ➔ **"Project"**.
3. Selecione o repositório que acabou de subir no GitHub.
4. A Vercel detectará automaticamente as configurações através do `vercel.json`:
   - **Framework Preset**: `Vite`
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
5. Clique em **"Deploy"**.
6. Pronto! Em menos de 30 segundos seu link estará no ar com HTTPS gratuito e CDN global.

---

## 💻 Como Rodar Localmente

### Opção A: Com Vite & Node.js
```bash
# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev

# Para gerar o build de produção
npm run build
```

### Opção B: Arquivo Único Standalone
Como o arquivo `index.html` foi construído de forma autocontida (com Tailwind e Lucide via CDN), você também pode simplesmente **dar um duplo clique no `index.html`** ou abri-lo diretamente em qualquer navegador sem precisar de Node.js instalado!

---

## 🛠️ Personalização Rápida

Todos os dados dos perfis estão concentrados no objeto `PROFILES` dentro do `<script>` no final do `index.html`:

- **Nome e Registro**: Altere `name`, `title` e `registry` (CRP, OAB, CRM, etc.).
- **Foto de Perfil**: Substitua a URL em `avatar` por sua foto hospedada ou link do Unsplash/Cloudinary.
- **WhatsApp**: Altere `whatsapp: "5511998765432"` com o seu DDI + DDD + número.
- **Chave Pix**: Modifique `pixKey` e `bank` para recebimento de honorários.
- **Endereço**: Ajuste `address` e `addressMapQuery` para o link automático do Google Maps.
- **Serviços**: Adicione, remova ou altere os cards na lista `services`.

---

## ✨ Recursos Inclusos

- [x] **Seletor de Tema Claro / Escuro Global**: Paleta creme/sálvia no modo claro e obsidiana/champagne no modo noturno com alto contraste.
- [x] **Alternância de Perfis (Psicologia Clínica & Advocacia)**: Modelo flexível para múltiplos nichos liberais.
- [x] **Agendamento Inteligente via WhatsApp**: Modal interativo com pré-seleção de modalidade e turno preferido.
- [x] **Chave Pix com Cópia Rápida**: Feedback visual instantâneo, alteração de estado do botão e vibração tátil (*haptics* no celular).
- [x] **Localização com Google Maps**: Botão direto "Como Chegar" e cópia de endereço.
- [x] **Download de Cartão de Visitas (.vcf)**: Salva o contato do profissional diretamente na agenda do smartphone.
- [x] **QR Code Dinâmico**: Ideal para cartões de visita físicos ou compartilhamento presencial.
- [x] **100% Responsivo & Mobile-First**: Perfeito no iPhone, Android e centralizado elegantemente no Desktop.

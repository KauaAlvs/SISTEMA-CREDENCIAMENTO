<div align="center">
  <img src="https://ik.imagekit.io/1t4v46udu/SA%C3%9ADE/LOGO%20PAPA%20MIKE%20SA%C3%9ADE.png" alt="Logo Papa Mike Saúde" width="250"/>
  <img src="https://ik.imagekit.io/1t4v46udu/SA%C3%9ADE/LOGO%20CEOZ.png?updatedAt=1779300255348" alt="Logo CEOZ" width="350"/>

  # 🛡️ Papa Mike Saúde | 2º CEOZ Sistema de Credenciamento & Auditoria
  
  **Segurança e agilidade na porta do seu evento.** <br>
  Plataforma de alta performance para validação de ingressos via código de barras, com monitoramento em tempo real e auditoria completa de acessos.

  ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
  ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
  ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
  ![Supabase](https://img.shields.io/badge/Supabase-181818?style=for-the-badge&logo=supabase&logoColor=3ECF8E)
  ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

</div>

---

## 📖 Visão Geral

O **Papa Mike - Módulo de Credenciamento** foi desenvolvido para solucionar gargalos críticos na recepção de eventos de grande escala. Através de um leitor de código de barras industrial/móvel e uma interface ultra-rápida, o sistema valida ingressos, previne fraudes por duplicidade e mantém um histórico de auditoria transparente para os gestores.

Desenvolvido com foco total em **UX para operadores de portaria**, o sistema garante que qualquer tentativa de acesso seja processada em milissegundos, com feedback visual claro e imediato.

---

## ✨ Funcionalidades Principais

### 🔍 Terminal de Check-in (Scanner)
- **Modo Scanner/Manual:** Suporte a leitores de código de barras via HID (teclado) e entrada manual de emergência.
- **Feedback Visual Premium:** Modal de status (Sucesso/Bloqueio) com design de alto contraste para leitura rápida à distância.
- **Prevenção de Duplicidade:** Bloqueio inteligente de ingressos já utilizados com exibição do horário exato do primeiro acesso.
- **Validação Temporal:** Verificação automática de permissões por dia do evento.

### 📋 Monitoramento e Auditoria
- **Dashboard de Logs:** Monitoramento em tempo real (polling a cada 10s) de todas as tentativas de acesso.
- **Rastreabilidade Total:** Registro persistente no banco de dados (`scan_logs`) de cada "bip", com status da ação e timestamp servidor.
- **Filtros de Segurança:** Busca rápida por código ou resultado, permitindo resposta imediata a intercorrências na portaria.

---

## 🛠️ Arquitetura Técnica

Utilizamos uma stack "Modern-Serverless" para garantir que o sistema não dependa de servidores pesados:

* **Framework:** [Next.js (App Router)](https://nextjs.org/)
* **Backend / Database:** [Supabase](https://supabase.com/) (PostgreSQL + RLS)
* **Performance:** [Vercel Edge Network](https://vercel.com/)
* **Proteção de DNS/CDN:** [Cloudflare](https://cloudflare.com/) (Gerenciamento de tráfego e SSL)
* **Estilização:** [Tailwind CSS](https://tailwindcss.com/) + [Lucide Icons](https://lucide.dev/)

---

## 🔐 Segurança & Performance
- **Isolamento de Dados:** Tabela de logs dedicada com RLS (Row Level Security) configurada para alta performance de escrita.
- **Estabilidade:** Infraestrutura distribuída entre Vercel e Cloudflare, garantindo que o sistema nunca saia do ar durante picos de público.
- **UX Adaptativa:** Interface pensada para tablets e smartphones, com "foco forçado" nos inputs para garantir que o leitor de código de barras esteja sempre pronto para o próximo ingresso.

---

## 🚀 Roadmap de Refinamento
- [ ] Otimização final do Design System do modal de acesso.
- [ ] Implementação de exportação de logs em CSV/Excel para auditoria offline.
- [ ] Adição de métricas de ocupação em tempo real no Dashboard.
- [ ] Refinamento das mensagens de bloqueio para suporte ao cliente.

---

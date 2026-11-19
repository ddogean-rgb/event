# Event — Marketplace de eventos (protótipo)

Projeto front-end React + Vite, responsivo e em português.

## Rodar localmente

1. Instale Node.js 20 ou superior.
2. Abra um terminal na pasta `event-marketplace`.
3. Execute `npm install`.
4. Execute `npm run dev`.
5. Abra o endereço local indicado no terminal (normalmente http://localhost:5173).

Para gerar a versão de publicação: `npm run build` (pasta `dist`).

## O que está implementado

- Homepage, busca, categorias, filtros e páginas de anúncios.
- Solicitação de reserva por data, carrinho e checkout simulado.
- Cadastro/login apenas demonstrativo, painel, publicação de anúncios, favoritos, mensagens locais e histórico de solicitações.
- Persistência no `localStorage` do navegador.

## Limitações importantes

- **Não há autenticação real.** O formulário de login aceita credenciais de demonstração e não valida identidade. Não use senhas verdadeiras.
- **Não há servidor nem banco de dados compartilhado.** Dados de um navegador não aparecem para outros usuários.
- **Não há pagamento real.** Pix e cartões são apenas seleções visuais.
- **Não há chat entre usuários em tempo real.** As mensagens são locais e não são enviadas a fornecedores.
- **Não há contrato assinado ou reserva confirmada.** A solicitação é um registro demonstrativo.
- **Os anúncios, imagens, preços e avaliações iniciais são ilustrativos.**
- O manifesto é apenas preparação inicial para PWA; ícones e service worker ainda precisam ser adicionados.

## Próximas integrações para produção

1. Supabase Auth com contas reais e autorização de acesso por usuário.
2. Supabase Postgres, Storage, políticas RLS e upload seguro de fotos.
3. Mensagens em tempo real com regras de acesso e notificações.
4. Calendário com disponibilidade, prevenção de reservas duplicadas e confirmação do fornecedor.
5. Provedor de pagamentos com suporte a split, webhooks, estornos e conciliação.
6. Contratos individualizados com revisão jurídica e serviço de assinatura eletrônica.
7. Políticas de privacidade, LGPD, moderação, antifraude, suporte e segurança.
8. Ícones, service worker, testes, acessibilidade e implantação para PWA.

## Publicação

O front-end está preparado para deploy estático em Netlify ou Vercel. Para ambiente comercial, as integrações acima são indispensáveis.

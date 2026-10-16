# PRD — RECOMEÇO 2.0

## 1. Visão e propósito
**Produto:** RECOMEÇO — Seu dinheiro, sua evolução.  
**Contexto:** desafio DIO App de Organização de Finanças Pessoais com Vibe Coding.  
**Modelo:** uso pessoal, acesso 100% gratuito, sem assinatura ou cobrança.  
**Demonstração:** https://sight-right-app.lovable.app/

## 2. Problema
Pessoas com contas acumuladas, dívidas e dificuldades de organizar o orçamento precisam de uma ferramenta simples que esclareça a situação atual e ajude a planejar os próximos passos. O controle isolado de despesas não basta quando existem parcelas, vencimentos e receitas futuras incertas.

## 3. Público
Pessoas com dificuldade financeira, endividadas, iniciantes em educação financeira e usuários que desejam melhorar hábitos sem receber julgamentos.

## 4. Objetivo do MVP
Permitir registrar contas, receitas, despesas e dívidas; consultar vencimentos; visualizar saldos realizados e previstos; e compreender ações prioritárias com linguagem acolhedora.

**Critérios de sucesso:** o usuário consegue inserir dados, entender quanto tem, quanto deve, quando as contas vencem e como uma decisão afetará o orçamento.

## 5. Funcionalidades e prioridade
| Prioridade | Recurso | Resultado esperado |
| --- | --- | --- |
| P0 | Contas, receitas, despesas | Lançamentos persistidos e categorizados |
| P0 | Dashboard | Valores reais, previstos e compromissos separados |
| P0 | Central de dívidas | Cadastro, vencimentos e acompanhamento |
| P0 | Segurança | Dados privados e controle de acesso |
| P1 | Calendário e cenários | Planejamento temporal e riscos de caixa |
| P1 | Simulador de compras | Impacto à vista ou parcelado |
| P1 | Simulador de quitação | Comparação sem inventar condições |
| P2 | Metas e evolução | Acompanhamento educativo |
| P2 | Meu mentor | Perguntas rápidas com regras financeiras |
| P2 | Relatórios e exportação | Autonomia e portabilidade |

## 6. Prompt final consolidado — briefing para Lovable

> Atue como equipe sênior de produto, UX, desenvolvimento full-stack, segurança e matemática financeira. Continue o projeto RECOMEÇO, preservando componentes, autenticação e banco existentes. Desenvolva um aplicativo pessoal e gratuito de organização e recuperação financeira, responsivo, em português brasileiro, com visual acolhedor verde-floresta, sem monetização ou planos pagos.
>
> Implemente contas financeiras, receitas, despesas, transferências, recorrências, cartões e dívidas. Crie dashboard com saldo realizado, receitas, despesas, compromissos futuros, dívidas, calendário e projeções de 7, 15, 30 dias e 3, 6 e 12 meses. Desenvolva uma central de dívidas com parcelamentos, propostas de negociação e comparação de estratégias avalanche, bola de neve e personalizada. Adicione o modo SOS, o simulador “Posso comprar?”, “Meu eu do futuro”, metas, jornada de evolução, relatórios e mentor educativo baseado inicialmente em regras, sem API paga.
>
> Utilize React, TypeScript e interface responsiva. Persistência preferencial em Supabase/PostgreSQL, com autenticação e RLS. Centralize o motor de cálculos em serviços testáveis, usando valores monetários exatos, evitando duplicações entre transferências, faturas, compras e pagamentos. Diferencie receitas previstas das recebidas, explicite hipóteses e nunca invente juros, acordos ou valores.
>
> Garanta privacidade, validação no servidor, backups/exportação e proteção de segredos. Não disponibilize cadastro público após configurar a conta proprietária. Reutilize o código existente, não faça perguntas intermediárias desnecessárias, não simule funcionalidades como prontas e não use dados fictícios como se fossem reais.
>
> Execute os módulos em ordem de dependência e informe ao final o que foi implementado, testado, parcial ou pendente, incluindo configurações externas. Priorize um MVP funcional e seguro em vez de muitas telas sem persistência.

## 7. Jornada sugerida
1. Diagnóstico amigável e cadastro gradual.
2. Registro de contas, ganhos e gastos.
3. Mapeamento das dívidas e obrigações essenciais.
4. Visualização do calendário e da projeção.
5. Comparação de alternativas e definição de ações.
6. Revisão semanal e acompanhamento de metas.

## 8. Requisitos não funcionais
- Interface mobile-first e acessível.
- Dados privados por usuário e login protegido.
- Cálculos determinísticos e testes financeiros.
- Não permitir que o assistente execute pagamentos.
- Backup e exportação de dados.
- Sem dependência obrigatória de serviço pago.

## 9. Validação e limites
O PRD documenta **o escopo solicitado à IA**. A implementação efetiva e os testes devem ser comprovados separadamente; a existência do site publicado não verifica, por si só, todas as funcionalidades.

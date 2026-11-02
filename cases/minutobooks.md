# Minutobooks

Insights de livros de não ficção para ler ou ouvir em cerca de 13 minutos,
com aplicativo para iOS, Android e web.

[Apresentação no portfólio](https://diogovieira.com.br/minutobooks) · [Site](https://minutobooks.com.br)

## A experiência

O Minutobooks reúne leitura e narração no mesmo catálogo. O acesso gratuito
inclui o Livro do Dia e uma estante semanal; a assinatura Pro amplia o acesso.
Um painel administrativo apoia a produção dos conteúdos com IA.

<img src="../assets/minutobooks.webp" width="320" alt="Player de áudio do Minutobooks, com capa, progresso e controles de reprodução">

*Captura da interface utilizada no portfólio. Representa o visual no momento do registro.*

## Decisões técnicas

| Necessidade | Abordagem |
| --- | --- |
| Atender celular e navegador | React Native com Expo e react-native-web, com módulos próprios para diferenças entre plataformas. |
| Vincular assinatura à conta | Validação no backend pela integração com RevenueCat, permitindo acesso entre plataformas. |
| Controlar o acesso ao áudio | URLs assinadas para narração e prévia pública limitada. |
| Organizar catálogo e conteúdo | API Express, Prisma e PostgreSQL, com Redis para estado temporário. |

**Stack:** TypeScript, React Native, Expo, Node.js, Express, Prisma,
PostgreSQL e Redis.

O repositório possui testes automatizados e portões locais de qualidade.
Esta apresentação não publica código, credenciais ou dados de usuários.

[Voltar ao perfil](../README.md)

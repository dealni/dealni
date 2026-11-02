# UpCanaisBot

Diretório de canais e grupos do Telegram com divulgação cruzada,
regras de participação e moderação de anúncios.

[Apresentação no portfólio](https://diogovieira.com.br/upcanais) · [Telegram](https://t.me/UpCanaisBot)

## A experiência

O bot reúne descoberta de canais, cadastro e participação na divulgação.
Os canais são organizados por faixa de inscritos; a participação pode render
pontos usados em anúncios sujeitos a moderação.

## Decisões técnicas

| Necessidade | Abordagem |
| --- | --- |
| Aplicar regras de participação | Verificação de posse e permissões, critérios de inscritos e fluxo de aprovação. |
| Organizar a divulgação | Faixas de inscritos e tratamento próprio para categorias com regras específicas. |
| Recuperar processamento interrompido | Registro do update em PostgreSQL antes da confirmação do webhook, com retomada por rotina agendada. |
| Moderar anúncios | Integração de IA pelo OpenRouter antes do envio. |

**Stack:** PHP, PostgreSQL, Redis, Monolog, Nginx e PHP-FPM.

O código usa análise estática, testes automatizados e testes de mutação.
O registro de updates permite retomar o processamento; efeitos externos
dependem do tratamento de cada operação.

[Voltar ao perfil](../README.md)

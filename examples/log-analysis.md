# Exemplo sintético — análise de logs

## Entrada

```text
10:02 login_failed user=demo source=203.0.113.10
10:03 login_failed user=demo source=203.0.113.10
10:04 login_success user=demo source=203.0.113.10
```

## Leitura defensiva

- há duas falhas seguidas de um sucesso para a mesma conta e origem;
- o padrão justifica validar autenticação, reputação da origem e atividade posterior;
- três eventos isolados não comprovam comprometimento;
- próximos passos: confirmar o proprietário da conta, revisar MFA e correlacionar com outros logs.

O endereço pertence ao bloco reservado para documentação e não representa um alvo real.

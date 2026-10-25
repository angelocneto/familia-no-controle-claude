# Família no Controle

![Farol do Família no Controle](assets/farol.png)

Registre despesas e receitas e consulte o placar da sua família na conversa com o Claude. A skill Farol no Claude orienta o uso das oito ferramentas do conector com os nomes, categorias e contas da sua família.

## Conexão

Você precisa de uma conta no [Família no Controle](https://app.familianocontrole.com.br). Para registrar jogadas, o acesso deve estar vigente. O Claude pode aplicar seus próprios limites de uso e regras da organização.

Este pacote está em preparação para o diretório. Enquanto a publicação não ocorrer, no Claude abra Personalizar, Conectores, +, Adicionar conector personalizado. Dê o nome Família no Controle e use este endereço:

```text
https://mcp.familianocontrole.com.br/mcp
```

Entre na sua conta e leia a autorização. A senha é digitada na tela do Família no Controle; o Claude recebe a autorização OAuth. Ative a conexão na conversa. O cadastro manual conecta as ferramentas; a skill faz parte da instalação deste pacote.

Confira o e-mail mostrado antes de autorizar. Use “Usar outra conta” se precisar trocar de família. O acesso será aos dados da família dessa conta.

## Experimente

- “Lança 45 no mercado, baú Família.” Se houver mais de uma conta possível, informe qual usar.
- “Quanto gastei com mercado em setembro de 2026?”
- “Como fechou agosto de 2026?”

## O que está disponível

| Ferramenta | Finalidade |
|---|---|
| `lancar_despesa` | Registrar uma despesa |
| `lancar_receita` | Registrar uma receita |
| `listar_baus` | Consultar baús e contas |
| `listar_pessoas` | Consultar pessoas e centros de custo |
| `consultar_saldo` | Consultar saldos |
| `listar_gastos_periodo` | Consultar jogadas por período |
| `resumo_do_mes` | Consultar receitas, despesas e grupos do mês |
| `listar_categorias` | Consultar categorias |

O conector não edita nem apaga jogadas, não cria categorias e não executa as análises do Farol. Ele não movimenta dinheiro, faz pagamentos, acessa bancos ou compra investimentos. Lançar uma jogada significa registrar um dado no seu controle financeiro.

## Dados e privacidade

O pacote contém instruções e a configuração de um único servidor remoto, com gateway na Cloudflare e dados no Supabase, em contas do Família no Controle. Não instala programas, não executa scripts locais e não precisa de chave de API. Não lê arquivos nem coleta o histórico da conversa.

Quando você pede uma ação, os campos necessários chegam ao servidor. As respostas podem conter valores, descrições, datas, categorias, baús, contas e pessoas da família, de acordo com a ferramenta. O Claude recebe essas respostas para atender ao pedido. Os lançamentos e registros de operação ficam no serviço Família no Controle; o pacote não cria um armazenamento local próprio. O tratamento da conversa no Claude segue as condições da sua conta Anthropic.

Consulte a [Política de Privacidade](https://familianocontrole.com.br/legal.html#privacidade), os [Termos de Uso](https://familianocontrole.com.br/legal.html#termos) e a [privacidade da Anthropic](https://www.anthropic.com/legal/privacy).

## Resolver dificuldades

Se a autorização expirar, reconecte em Configurações, Conectores no Claude. Para interromper o acesso, desconecte por esse mesmo local. Se uma escrita tiver resultado incerto, confira as Jogadas no app antes de repetir. Para dados, exclusão da conta ou dúvidas sobre acesso e retenção, use o suporte.

Suporte: [contato@familianocontrole.com.br](mailto:contato@familianocontrole.com.br).

## Licença e versão

Versão 0.1.1, ainda não publicada. Textos e configurações sob licença MIT, aprovada pelo titular em 26/09/2026. A marca e o ícone mantêm os direitos reservados e a permissão limitada descrita em LICENSE.

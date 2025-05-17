# imersaoalura
Projeto de final de imersão de 2025

Agentes de Medicamento

Quem nunca se viu perdido após uma consulta médica, sem lembrar exatamente para que serve aquele medicamento receitado? A proposta aqui é criar uma ferramenta capaz de fornecer informações cruciais sobre um dado remédio, como sua indicação terapêutica, modo de uso, a faixa de preço praticada no mercado, possíveis efeitos colaterais, a disponibilidade de um correspondente genérico e a respectiva variação de preço.

Aspectos Técnicos:

Entrada:
- Nome do medicamento

Saída:
- Nome do medicamento completo
- Indicação terapêutica
- Posologia e modo de uso
- Faixa de preço do medicamento original
- Possíveis efeitos colaterais
- Disponibilidade de genérico: Sim/Não
- Faixa de preço do medicamento genérico (se disponível)

Arquitetura:
- Agente 1, Agente 2 => Redator => Revisor

Agente de Busca ANVISA: Encarregado de consultar a base de dados da Agência Nacional de Vigilância Sanitária (ANVISA) para obter informações oficiais sobre o medicamento, como indicação, uso e efeitos colaterais.
Agente de Busca de Preços: Responsável por pesquisar em diversos sites de e-commerce e farmácias online para coletar dados sobre a faixa de preço do medicamento original dos últimos 5 meses e, se disponível, do genérico.
Redator: Utiliza as informações coletadas pelos Agentes de Busca para gerar um descritivo claro e acessível para o usuário leigo, evitando termos técnicos complexos.
Revisor: Realiza uma verificação ortográfica e de "temperatura" (garantindo que a linguagem seja adequada e amigável) do texto produzido pelo Redator antes de ser apresentado ao usuário.

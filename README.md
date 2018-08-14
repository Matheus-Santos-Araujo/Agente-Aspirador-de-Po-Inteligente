# Agente-reflexivo-simples-Aspirador-de-p-
Trabalho básico de IA

Detalhes de PEAS

O agente não tem total ciência do ambiente. Só capta e aspira a sujeira de uma área. Move-se
aleatoriamente para verificar a existência de sujeira, sem se preocupar com energia perdida.
São apenas 2 áreas, para N áreas é necessário criar uma proporção dos objetos da tela (para 
curiosidade) e, para melhor visualização de simulação, novas imagens de fundo (drawings) ou 
divisão de fundo (patches) feita por cores-contraste. São utilizadas poucas regras e o 
desenvolvimento do ambiente (ficar sujo) é aleatório - Tendo o agente, como única atuação 
sobre ele, "negar" a sujeira.

Podemos dizer que o ambiente deste agente é: Parcialmente observável, Determinístico, Episódico, Discreto, Conhecido e possuí apenas um agente.

S=>Sujo;
E=>Está em;
L=>Aspirar;
M=>Mover para;
1/2=>Áreas A/B;

(S1/\E1->L1/\M2)/\(L1/\E1->M2)/\(S2/\E2->L2/\M1)/\((L2/\E2)->M1)

Alterações de complexidade sugeridas:

Tornar ambiente completamente observável e definir uma medida de eficiência (performance).
Tornar ambiente estocástico criando uma chance de Sugar/Limpar não ser 100% eficiente.
Tornar o ambiente sequencial utilizando métodos de busca para decisões futuras(afeta performance).

Sobre o agente:

Criar tempo máximo de utilização e/ou bateria.
Desgaste do atuador(aspirador).

RM: 570072
Publicado em: (https://cp1-tailwind-isaac.vercel.app/)
Carta: 03 · Papel & Tinta

IA: pedi ao Claude para estilizar o index.html travado com Tailwind seguindo
minha carta (fundo #F7F4ED, tinta #211E1A, destaque #7A2E2E, Playfair Display
+ Source Sans 3, raio 2px). Ele montou o @theme e as classes do header, hero,
lista de dados e rodapé. Depois de testar, encontrei um bug de scroll horizontal
na página inteira causado pelo header (logo e botão disputando espaço no
mobile) e pedi correção — a solução foi trocar o header para flex-col por
padrão e só virar flex-row a partir do sm. Também pedi para deixar o scroll
horizontal da lista de dados (Data/Local/Ingressos) mais intencional; em vez
de esconder a barra de rolagem com CSS (o que violaria a regra 5, de não usar
CSS fora do @theme), usei snap-x/snap-start, que são utilitários nativos do
Tailwind.

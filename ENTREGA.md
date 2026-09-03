# Entrega - Checkpoint 1

## Identificacao

**RM:** 573599  
**Aluno:** Heitor Anacleto  
**Carta:** 25 - Turno  
**Tema:** Feira de gastronomia noturna  
**Adjetivos da carta:** tardio, eletrico e urbano  
**Data da entrega:** 03/09/2026  

## Links da entrega

**Repositorio publico no GitHub:** COLE_AQUI_O_LINK_DO_GITHUB  
**Projeto publicado na Vercel:** COLE_AQUI_O_LINK_DA_VERCEL  

Os dois links acima devem ser preenchidos antes do envio do assignment do Teams.
O projeto deve abrir normalmente em uma aba anonima do navegador.

## Descricao do projeto

Este projeto e uma landing page para o evento Turno, uma feira de gastronomia
noturna. A identidade visual segue a Carta 25, com uma linguagem tardia,
eletrica e urbana.

O projeto foi desenvolvido no arquivo `index.html`, usando HTML semantico e
utilitarios do Tailwind CSS v4. O Tailwind e carregado pelo script fornecido no
arquivo, sem necessidade de instalar dependencias, usar npm ou configurar um
processo de build.

## Regras respeitadas

- A estrutura original do `body` foi mantida.
- Foram adicionadas classes Tailwind aos elementos existentes.
- Os textos do evento foram personalizados para a carta Turno.
- As fontes e os tokens foram declarados na area editavel do `head`.
- Nao foi utilizado CSS proprio fora do bloco `@theme`.
- Nao foram utilizados valores arbitrarios do Tailwind.
- O layout foi construido com abordagem mobile-first.

## Tokens da Carta 25

```css
@theme {
	--color-marca-50:  #14141A;
	--color-marca-900: #F5F5F0;
	--color-marca-500: #E4FF3A;
	--font-display: "Antonio", sans-serif;
	--font-corpo: "Manrope", sans-serif;
	--radius-card: 2px;
}
```

### Cores

- `#14141A` e o fundo da pagina e foi usado com `bg-marca-50`.
- `#F5F5F0` e a tinta dos textos, bordas e botoes claros e foi usado com
	`text-marca-900`.
- `#E4FF3A` e a cor de destaque dos rotulos e do botao principal e foi usada
	com `bg-marca-500`.

### Tipografia

- `Antonio` foi usada nos titulos e nos dados de destaque com `font-display`.
- `Manrope` foi usada nos textos corridos e na navegacao com `font-corpo`.
- As fontes sao carregadas pelo Google Fonts no `head`.

### Raio

- O raio definido foi de `2px`.
- O token `--radius-card` gera o utilitario `rounded-card`, usado nos botoes.

## Responsividade

A pagina segue a regra de composicao da carta:

- No mobile, os dados de data, local e ingressos ficam empilhados em uma coluna
	com `grid-cols-1`.
- A partir do breakpoint `sm`, os dados ficam em tres colunas iguais com
	`sm:grid-cols-3`.
- O cabecalho usa `flex` e esconde a navegacao em telas pequenas com
	`hidden md:block`.
- O rodape muda de coluna para linha a partir do breakpoint `md`.
- Os botoes usam `flex-wrap` para continuarem acessiveis em telas estreitas.

## Estados e acessibilidade

- Os links e botoes possuem estados de interacao com `hover:`.
- Os links e botoes possuem foco visivel com `focus-visible:outline-2`.
- O texto claro sobre o fundo escuro atende a orientacao de contraste da ficha.
- O texto sobre o destaque usa a cor do fundo, e nao branco, conforme o aviso
	da Carta 25.
- A pagina utiliza elementos semanticos como `header`, `nav`, `main`, `section`,
	`dl`, `dt`, `dd` e `footer`.

## Checklist antes do envio

- [ ] Repositorio do GitHub publico.
- [ ] Link do GitHub preenchido neste arquivo.
- [ ] Projeto publicado na Vercel.
- [ ] Link da Vercel preenchido neste arquivo.
- [ ] Link da Vercel testado em uma aba anonima.
- [ ] Pelo menos 3 pushes realizados.
- [ ] Intervalo de pelo menos 30 minutos entre o primeiro e o ultimo push.
- [ ] Nenhum push realizado depois das 09:40.
- [ ] `ENTREGA.md` esta na raiz do repositorio.
- [ ] Projeto testado em tela mobile e desktop.
- [ ] Declaracao de uso de IA preenchida abaixo.

## Declaracao de uso de IA

IA: usei o Gemini para me ajudar a separar o que precisava ser modificado no
projeto, como cores, espacamento, posicao e fonte. Tambem usei o GitHub Copilot
para revisar o codigo, entender o aviso do VS Code sobre a diretiva `@theme` e
conferir se o `index.html` seguia as regras do professor. Mantive a estrutura
original, apliquei os valores da minha ficha e conferi as classes utilizadas.

## Defesa

Na defesa, consigo explicar que `font-display` aplica a fonte Antonio aos
titulos, enquanto `font-corpo` aplica Manrope aos textos. Tambem consigo
explicar que `sm:grid-cols-3` transforma a lista de dados em tres colunas a
partir do breakpoint `sm`, mantendo uma coluna no mobile.
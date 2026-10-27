# Landing page — Recanto Flamboyant

Atualizado em 27/10/2026. Página: `site/index.html` (versão 4, com logo, fotos originais e
vídeo). Versões antigas em `site/_antigas/` (não publicar essa pasta).
Objetivo único: abrir conversa no WhatsApp.

## Fonte dos fatos
FICHA.md (casa), REGIAO.md (cidade), pecas/2026-10-27-precos-e-pacotes.md (preços e regras),
marca/tokens.css e marca/IDENTIDADE.md (cores, fonte, logo). A página não contradiz esses
arquivos. Texto do usuário (27/10) revisado pelas regras: sem endereço exato, sem adjetivos
não verificáveis ("escolha definitiva", "absoluta estrutura", "premium", "profissional"),
sem as colunas internas "Estratégia de mercado" e "Perfil do hóspede".

## Estrutura

| # | Seção | Conteúdo | Gatilho |
|---|---|---|---|
| 1 | Topo | Flor do logo, nome, "Casa de praia · Guaratuba (PR)", promessa, botão; foto D38 (piscina do alto) | redução de risco (sinal até 30/11) |
| 2 | Datas | "Uma casa, um grupo por vez": Natal, Réveillon, jan/fev, Carnaval, Páscoa + "Atualizado em" | escassez real |
| 3 | O nome | "A casa debaixo do flamboyant" (foto D03, sem o número) + "Mais que uma casa, um refúgio." | identidade |
| 4 | Lazer | "A praia aqui é opção": vídeo de 7 s da piscina, piscina 3×6, área gourmet, sala de jogos/TV, 3 fotos | experiência |
| 5 | A casa | 20 pessoas, 6 quartos (2 suítes), 4 banheiros, 6 vagas + comodidades + 8 fotos | prova concreta |
| 6 | Localização | "Longe do barulho, perto de tudo": 4 min / 1,8–2 km + comércio do bairro | conveniência |
| 7 | Guaratuba | Praia Central, Morro do Cristo, Caieiras, Igreja Matriz, guarás + bloco da Páscoa com maratona | região |
| 8 | Preços | Simulador (período, pacote ou diárias, pessoas → total, por pessoa, sinal, caução, mensagem pronta) + 3 tabelas | ancoragem por pessoa |
| 9 | Reserva | Sinal e cancelamento por período, como funciona, combinados da casa | segurança |
| 10 | Perguntas | Endereço, toalha, ar, pet, piscina e crianças, silêncio, visitas, idosos, carro | objeções |
| 11 | Fim | "O Réveillon tem uma noite só" + botão | escassez real |
| — | Rodapé | Logo, bairro, créditos das fotos da cidade | — |

## Preços (iguais à calculadora orcamento.py)
- Natal 24–27/12: R$ 7.500 · Réveillon 27/12–03/01: R$ 18.900 · Natal + Réveillon: R$ 24.000
- Jan/fev: 2 diárias R$ 1.800; 3–4 R$ 1.600; 5–6 R$ 1.500; 7+ R$ 1.400 (2–4 só com sexta e sábado)
- Carnaval 05–10/02: R$ 11.000 · Páscoa 25–28/03: R$ 6.000
- Limpeza R$ 400 · Caução R$ 1.500 · Sinal 50% (feriados) ou 30% (jan/fev)

## Mensagens do WhatsApp
- `?origem=grupo|instagram|facebook` → "Oi! Vi a casa Recanto Flamboyant pelo grupo (…) e queria saber das datas."
- Sem origem → "Oi! Vi a página da casa Recanto Flamboyant e queria saber das datas."
- Simulador → "… Quero saber de Réveillon (27/12 a 03/01), 7 diárias, 20 pessoas (estimativa do site: R$ 19.300 com limpeza)."

## Como atualizar
- Reserva fechada: trocar "livre" e a data de "Atualizado em" na seção Datas.
- Preços: mudar a tabela HTML e o objeto `PACOTES` / `diariaVerao` no script.
- Número do WhatsApp: variável `NUMERO` no script (só dígitos, com 55 e DDD).
- Domínio: trocar `SEU-DOMINIO` em `og:image` e `og:url`. Prévia: `og.jpg` (arte do designer).

## Fotos e vídeo
- Casa: originais de 28/12/2025 (fotos/drive-2025-12-28) e D03 de fotos/publicar. Não usadas:
  D04 (número 221), pernas na escada, colchão sem lençol.
- Vídeo: 7 s de 20251228_124619.mp4 (60–67 s), sem som, 1,7 MB, só toca quando aparece e
  nunca para quem pede menos movimento.
- Cidade (Wikimedia Commons), créditos no rodapé: Praia Central (Adiascamargo, CC BY-SA 4.0),
  Morro do Cristo (Glaucia Paes, CC BY-SA 3.0), Caieiras e Igreja Matriz (Renato Soares/MTur,
  domínio público), Revoada dos guarás (TropoPiegas, CC BY-SA 4.0).

## Pendências antes de publicar
- [x] 2 suítes (confirmado em 27/10)
- [x] Ventilador de teto em todos os quartos, menos a suíte master (que tem ar-condicionado)
- [x] Sem videochamada: o passo saiu da página
- [x] WhatsApp: número no script (variável NUMERO)
- [ ] Aprovar as regras de sinal, caução e cancelamento (explicadas ao usuário em 27/10)
- [ ] Domínio e publicação (item D)

## Verificação de 27/10/2026
- Inspetor taste: 0 FAIL, 0 WARN em 1440, 768 e 390 (exceções da marca: paleta creme +
  vermelho e assinatura em caixa-alta).
- Lighthouse celular: acessibilidade, boas práticas e SEO 100.
- Simulador conferido com a tabela em 8 cenários; links de WhatsApp por origem; menos movimento.
- Revisão de design do designer (design/revisoes/2026-10-27-landing-page.md): 7 ajustes aplicados.

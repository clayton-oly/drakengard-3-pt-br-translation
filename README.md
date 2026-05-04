# Drakengard 3 PT-BR

Patch em PT-BR para `Drakengard 3` de PS3.

## Compatibilidade testada

- `BLUS31197`
- jogo em formato de pasta (`PS3_GAME`, `PS3_UPDATE`, `PS3_DISC.SFB`)
- RPCS3 com `Unprotect game files` ativado

## Status da traducao

- cobertura atual: `100%` das linhas dos CSVs do projeto-base (`16879/16879`)
- capitulos traduzidos: prologo/Capitulo 0 ate Capitulo 5, incluindo versos/cenas extras disponiveis nos CSVs do projeto-base
- menus principais, opcoes, pause menu, tutoriais, resultado, selecao/preparacao de capitulos e banco de dados de personagens
- missoes, objetivos, condicoes de quest, textos comuns usados durante a campanha, itens, armas, efeitos, historias de armas, nomes de monstros, dicas de chefes, DLCs, staff roll e textos de gameplay
- nomes genericos exibidos em missoes foram normalizados, como `Soldier A` para `Soldado A`
- resumos da selecao de missoes do Capitulo 3 foram revisados onde ainda havia texto em ingles

## Ainda pendente

- revisao de textos longos que podem sair da area da tela

## Observacoes

- os textos foram gerados a partir dos CSVs do projeto Arekushi e aplicados na ordem oficial de `_export.json`
- os textos foram normalizados sem acentos para evitar caracteres quebrados na build testada
- a build foi aplicada em lotes e testada no RPCS3 durante o Capitulo 2
- este repositorio distribui apenas o patch, nao os arquivos completos do jogo

## Arquivos do patch

- `patch/ALLMESSAGE_SF.XXX`
- `patch/MISSIONMESSAGE_SF.XXX`
- `patch/PS3TOC.TXT`

## Como instalar

1. Tenha uma copia limpa de `Drakengard 3` (`BLUS31197`) em formato de pasta.
2. Entre em `PS3_GAME/USRDIR/SQEX03GAME/`.
3. Faca backup destes arquivos originais:
   - `COOKEDPS3/ALLMESSAGE_SF.XXX`
   - `COOKEDPS3/MISSIONMESSAGE_SF.XXX`
   - `PS3TOC.TXT`
4. Copie os arquivos da pasta `patch/` deste repositorio para os destinos abaixo:
   - `patch/ALLMESSAGE_SF.XXX` -> `PS3_GAME/USRDIR/SQEX03GAME/COOKEDPS3/ALLMESSAGE_SF.XXX`
   - `patch/MISSIONMESSAGE_SF.XXX` -> `PS3_GAME/USRDIR/SQEX03GAME/COOKEDPS3/MISSIONMESSAGE_SF.XXX`
   - `patch/PS3TOC.TXT` -> `PS3_GAME/USRDIR/SQEX03GAME/PS3TOC.TXT`
5. No RPCS3, ative `Unprotect game files`.
6. Se o jogo ja criou dados em `dev_hdd0/game/BLUS31197DATA`, copie tambem:
   - `patch/ALLMESSAGE_SF.XXX` -> `dev_hdd0/game/BLUS31197DATA/USRDIR/FIOS-UNREALENGINE3/SQEX03GAME/COOKEDPS3/ALLMESSAGE_SF.XXX`
   - `patch/MISSIONMESSAGE_SF.XXX` -> `dev_hdd0/game/BLUS31197DATA/USRDIR/FIOS-UNREALENGINE3/SQEX03GAME/COOKEDPS3/MISSIONMESSAGE_SF.XXX`
   - `patch/PS3TOC.TXT` -> `dev_hdd0/game/BLUS31197DATA/USRDIR/FIOS-UNREALENGINE3/SQEX03GAME/PS3TOC.TXT`
7. Abra o jogo.

## Como remover

Restaure os 3 arquivos originais do seu backup:

- `COOKEDPS3/ALLMESSAGE_SF.XXX`
- `COOKEDPS3/MISSIONMESSAGE_SF.XXX`
- `PS3TOC.TXT`

## Nota importante

Aplicar este patch em instalacoes diferentes, dumps diferentes ou estruturas diferentes do jogo pode causar travamentos. O metodo mais seguro e usar uma copia limpa em formato de pasta. No RPCS3, se o jogo travar apos atualizar os `.XXX`, confira se o `PS3TOC.TXT` tambem foi copiado para o cache `BLUS31197DATA`.

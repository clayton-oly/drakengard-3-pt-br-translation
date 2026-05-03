# Drakengard 3 PT-BR

Patch parcial em PT-BR para `Drakengard 3` de PS3.

## Compatibilidade testada

- `BLUS31197`
- jogo em formato de pasta (`PS3_GAME`, `PS3_UPDATE`, `PS3_DISC.SFB`)
- RPCS3 com `Unprotect game files` ativado

## O que ja esta traduzido

- menu principal
- opcoes e configuracoes
- pause menu
- tutoriais
- nomes e objetivos basicos
- comeco da historia
- primeiros blocos como `M_0010`, `M_0020`, `M_1011` e `C_00`

## Observacoes

- este patch ainda nao traduz o jogo inteiro
- varios textos foram normalizados sem acentos para evitar caracteres quebrados na build testada
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
6. Abra o jogo.

## Como remover

Restaure os 3 arquivos originais do seu backup:

- `COOKEDPS3/ALLMESSAGE_SF.XXX`
- `COOKEDPS3/MISSIONMESSAGE_SF.XXX`
- `PS3TOC.TXT`

## Nota importante

Aplicar este patch em instalacoes diferentes, dumps diferentes ou estruturas diferentes do jogo pode causar travamentos. O metodo mais seguro e usar uma copia limpa em formato de pasta.

Link: https://x.com/agpatriota/status/2022358282250113520

Precisei incluir o Qualis e SJR no scriptlattes (
@jmenac
) que atualmente não está fazendo isso (pelo menos não vi como). 

Chatgpt 5.2 me deu um patch simples para editar alguns arquivos automaticamente:

patch -p1 < patch_qualis_sjr_scriptLattes.patch

que faz o seguinte:

1. cria scriptLattes/qualis_sjr.py
2. modifica scriptLattes/grupo.py
3. modifica scriptLattes/geradorDePaginasWeb.py

Agora basta incluir no topo do arquivo.list os arquivos contendo o qualis e o sjr:

@qualis=QUALIS2026.csv
@sjr=scimagojr 2024.csv

Ao rodar
python3 http://scriptLattes.py exemplo/file.config 

temos o resultado esperado. Espectacular.


![HBDcAR9aMAAOezr](https://github.com/user-attachments/assets/02c03f9b-ff3c-491a-880a-8877575f952a)


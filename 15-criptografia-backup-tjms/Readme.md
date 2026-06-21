**Prova TJM SP**

Para ampliar a segurança de arquivos de backup armazenados, pode-se encriptá-los. Considere o seguinte procedimento:

• O usuário gera um par de chaves pública/privada (chamadas aqui de **Pub/Priv**) por meio de um aplicativo utilitário de criptografia.

• A cada backup realizado, o usuário gera uma chave simétrica aleatória (**SymKey**) e encripta o arquivo de backup com ela. **SymKey**, por sua vez, é encriptada utilizando a chave **Pub**, gerando um texto cifrado (**SymKeyCipher**). **SymKey** e o arquivo de backup original são então descartados, e **SymKeyCipher** é armazenada junto com o arquivo de backup encriptado.

Nesse contexto, responda ao que se pede:

**a) Dentre as chaves criptográficas citadas, indique qual chave é utilizada para decriptar SymKeyCipher quando necessário recuperar um backup.**

**b) Caso os arquivos de backup e seus SymKeyCipher (apenas esses dados) sejam obtidos indevidamente por outra pessoa, indique se os conteúdos originais dos backups correm risco prático de serem revelados. Justifique.**

**c) Explique por que o usuário não poderia, ou não seria recomendado, encriptar seus arquivos de backup diretamente com a chave Pub.**

É necessário realizar a leitura de um arquivo texto, e trabalhar com o armazenamento das palavras do texto em estruturas encadeadas para gerar o índice remissivo. A figura a seguir apresenta um exemplo dessa representação: as palavras estão na lista vertical em ordem alfabética crescente e à cada uma delas está associada uma lista das páginas onde ocorrem.
Ao final do processamento o programa deverá apresentar a lista de palavras do texto ordenadas em ordem alfabética crescente e apresentando as páginas onde a palavra ocorreu no texto. Para facilitar, será considerado que a cada 40 linhas começa uma nova página. 

*Desenvolvimento*
O primeiro passo para a realização desse trabalho é ler o arquivo e obrigatoriamente criar estruturas encadeadas, capazes de guardar as palavras presentes no arquivo, juntamente com os números das páginas em que cada palavra aparece. O código para leitura de arquivos do tipo texto está disponível no Moodle, sendo necessário integrá-lo à sua solução.
Durante a leitura, é importante:
• Converter todas as palavras para minúsculas, para evitar duplicações desnecessárias;
• Remover qualquer sinal de pontuação no momento de armazenar a palavra;
• Identificar as stopwords e não armazená-las na lista;
• Inserir a ocorrência da palavra na lista e a página onde ocorreu.
Stopwords são palavras que podem ser consideradas irrelevantes para o resultado esperado. Por exemplo, no índice remissivo que será gerado não se espera encontrar palavras como “a”, “and”, “etc”, “my” e “the”. Portanto, um arquivo com as stopwords que devem ser ignoradas também foi disponibilizado no Moodle (veja o arquivo StopWords-EN.txt). Também existe um arquivo equivalente em português (StopWords-PT.txt).
É importante lembrar que se deve projetar uma forma de armazenamento das palavras que permita um rápido acesso a cada palavra, uma vez que antes de incluir cada palavra deve-se verificar se ela já não foi armazenada. Caso a palavra já exista, o programa deve apenas acrescentar mais um número de página onde ela aparece.
Lembre que uma palavra pode aparecer mais de uma vez em uma página, mas no índice remissivo não pode aparecer o mesmo número de página duas vezes.
Ao ser iniciado, o programa deverá solicitar o nome do arquivo de texto a ser processado. Ao concluir a leitura do arquivo, deve apresentar as funcionalidades a seguir em um menu em modo texto para o usuário:
1. Exibir todo o índice remissivo (em ordem alfabética);
2. Exibir o percentual de stopwords do texto (quanto % do texto é formado por stopwords);
3. Encontrar a palavra mais frequente, isto é, com maior número de ocorrências;
4. Pesquisar palavras, isto é, o usuário informa uma palavra e o programa lista os números das páginas em que a palavra ocorre;
5. Encerrar o programa.
O programa deve permitir que usuário execute qualquer das funções novamente, até que seja encerrado.

*Implementação*
Para a implementação é obrigatório o uso das classes fornecidas no arquivo CodigoBase.zip. Estas classes são descritas a seguir:
• ArquivoTexto: classe que encapsula o acesso ao arquivo que contém o texto;
• LinhaTexto: representa uma linha lida do arquivo. Esta classe possui um método que retorna cada uma das palavras da linha;
• ListaOrdenadaDePalavras: representa a lista de palavras existentes no arquivo;
• ListaDeOcorrencias: representa a lista encadeada de ocorrências de uma palavra.
O programa main, também fornecido juntamente com as classes, exemplifica como fazer a leitura de um arquivo texto.
É importante ressaltar que não podem ser utilizadas classes das API de coleções, como ArrayList, LinkedList, HashMap, HashSet, de Java.
As classes de lista vistas em aula podem servir como base para as estruturas de dados a serem desenvolvidas e utilizadas.

Esse trabalho realizei em 2023/2 na disciplina de Algoritmos e Estrutura de Dados I (ALEST I) ministrada pela profa. Isabel Harb. Esse trabalho fiz individualmente, no qual por meio dele consegui ampliar meus conhecimentos.

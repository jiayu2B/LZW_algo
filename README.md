Le programme lzw.py utilise deux méthode pour la compression / décompression LZW.
La première utilise l'ASCII étendue et la seconde le binaire.

L'ASCII étendu se fait sur 16 bits, est plus simple à implémenté mais est plus lent et moins performant en terme de décompréssion.
Passer par le binaire permet une compression / décompression plus rapide et plus efficace mais est bien plus complexe à mette en place.

Dans tous les cas l'ASCII étendue utilise aussi du binaire. Le fait d'écrire les caractères étendue dans un fichier texte, le type de fichier "texte" le convertie tous seul en hexa, sinon il serait illisible.
C'est pour ça que la méthode de l'ASCII étendue est plus simple à mettre en place, il y a une couche d'abstraction supplémentaire. Mais c'est aussi pourquoi elle est plus lente, les opérations binaires sont plus facile à faire pour l'ordinateur, pas pour l'humain.


Utilisation
===================

python3 ./lzw.py

LZW compressor / uncompressor
Choose an action to perform : 
[1] - Compress
[2] - Uncompress
> 1

=> Les fichiers compressés sont placés dans genFiles

LZW compressor / uncompressor
Choose an action to perform : 
[1] - Compress
[2] - Uncompress
> 2

=> Les fichiers décompressés sont placés dans genFiles

Le fichier texte de départ contient les 10000 premiers nombres premiers (10000.txt).
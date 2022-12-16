# SHA

- a sigla SHA (Secure Hash Algorithm), traduzindo, algoritmo de hash seguro. É um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA), algoritmo de encriptação.

  SHA1 vai pegar seu arquivo (foto, imagem, frase...) e vai embaralhar esse algoritmo, de uma forma bem especifica.

  A encriptação gera um conjunto de caracteres identificador de 40 digitos (identificação). É uma forma curta de representar o estado de um arquivo.

    					Exemplo: 

  ## 1 echo "ola mundo" | openssl sha1

  ## 2 > (stdin) = f9fc856o654...

# Objetos fundamentais: blobs, trees, commits

- As tree armazenam blobs \o (aponta para um blob ou outra tree)
- Os blobs só guardam o SHA do arquivo
- As tree monta toda a estrutura de onde está os arquivos



​						![objetosfundamentais](https://user-images.githubusercontent.com/101298597/207999634-a22ff7a1-0315-4379-82e6-d95d75982b2d.png)



- O commit (objeto) vai juntar tudo, e vai dar um "sentido" a alteração que fazemos.
- O commit aponta para uma tree, um parente (ultimo commit realizado antes dele), aponta para um autor, e para uma mensagem. Obs.: o autor e a mensagem fazem parte dessa ideia de sentido.

![commit](https://user-images.githubusercontent.com/101298597/208000482-b711ecd0-b889-4fb8-b79a-98deec1383df.png)

​																O SHA1 desse commit é o hash de toda essa informação

# 				Estado dos arquivos (Ciclo de vida)

![estadodosarquivos-noseuciclodevida](https://user-images.githubusercontent.com/101298597/208002551-d1cc1a0d-6c52-42ec-82f2-1d603f9f28c2.png)














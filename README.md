# RSA
A aplicação implementa a criptografia assimétrica pelo algorítmo RSA. O programa irá realizar a leitura de um arquivo de texto e se necessário dois arquivos de chave privada (d.txt n.txt). Ele retorna um novo arquivo com o prefixo "encrypted"/"decrypted" + nome do arquivo de input original. 


## Plataforma utilizada
20.04.2 LTS (Focal Fossa) (WSL)


## Funções:
- 1 : Modo de demonstração, o programa irá criar um par de chaves públicas e privadas, criptografar e descriptografar um arquivo de entrada
- 2 : Modo de criptografia, o programa irá criar um par de chave públicas e privada (d.txt n.txt) e criptografar um arquivo de entrada
- 3 : Modo de descriptografia, o programa irá ler dois arquivos de chave privada (d.txt n.txt) e descriptogrfar um arquivo de entrada (Para esse modo funcionar é necessário que os arquivos d.txt e n.txt existam)

## Execução
Para execução é necessário ter todos os arquivos utilizados na mesma pasta

Comando:
```
python main.py  <modo> <nome_arquivo> 
```


substitua <modo> por "1", "2" ou "3". <br>
Digite os parâmetros sem <>. <br>

### Exemplo:
1. Criptografando e descriptografando arquivos no modo demonstração: <br>
Em uma pasta com os arquivos teste.txt 

```
python main.py 1 teste.txt

cat encrypted_teste.txt

cat decrypted_teste.txt

```

2. Criptografando e descriptografando arquivos nos modos 2 e 3: <br>
Em uma pasta com os arquivos example_input.txt e example_key.txt 

```
python main.py 2 teste.txt

python3 main.py 3 encrypted_teste.txt

cat decrypted_encrypted_teste.txt

```

## Bibliotecas
- random
- sys








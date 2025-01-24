# Ransomware Simulation Scripts

Este repositório contém dois scripts Python que simulam o processo de criptografia e descriptografia de arquivos usando o módulo `pyaes`. **Estes scripts são apenas para fins educacionais e de estudo. Não use para atividades maliciosas.**

## Descrição dos Arquivos

### 1. `encrypt.py`
Este script criptografa um arquivo especificado usando AES (Advanced Encryption Standard) no modo CTR. O arquivo original é removido e substituído por uma versão criptografada.

#### Funcionamento:
1. Abre o arquivo `teste.txt` para leitura.
2. Lê os dados do arquivo.
3. Remove o arquivo original (`teste.txt`).
4. Define uma chave de criptografia (`testeransomwares`).
5. Criptografa os dados do arquivo.
6. Salva os dados criptografados em um novo arquivo com o nome `teste.txt.ransomwaretroll`.

---

### 2. `decrypt.py`
Este script descriptografa o arquivo gerado pelo `encrypt.py` usando a mesma chave de criptografia. O arquivo criptografado é removido e substituído por uma versão descriptografada.

#### Funcionamento:
1. Abre o arquivo `teste.txt.ransomwaretroll` para leitura.
2. Lê os dados criptografados.
3. Define a mesma chave de criptografia usada no `encrypt.py` (`testeransomwares`).
4. Remove o arquivo criptografado (`teste.txt.ransomwaretroll`).
5. Descriptografa os dados e salva em um novo arquivo chamado `teste.txt`.

---

## Dependências

- Python 3.x
- Módulo `pyaes`

### Instalação do `pyaes`:
Execute o comando abaixo para instalar a biblioteca:

```bash
pip install pyaes
```

---

## Como Usar

### 1. Criptografar um Arquivo
1. Certifique-se de ter um arquivo chamado `teste.txt` no mesmo diretório do script.
2. Execute o script `encrypt.py`:

   ```bash
   python3 encrypt.py
   ```

3. Após a execução, o arquivo `teste.txt` será substituído por `teste.txt.ransomwaretroll`.

---

### 2. Descriptografar um Arquivo
1. Certifique-se de ter o arquivo `teste.txt.ransomwaretroll` gerado pelo `encrypt.py` no mesmo diretório.
2. Execute o script `decrypt.py`:

   ```bash
   python3 decrypt.py
   ```

3. Após a execução, o arquivo `teste.txt.ransomwaretroll` será substituído por `teste.txt`.

### 3. Resultado
1. Arquivo de texto
   
![imagem do arquivo de texto](https://github.com/VictorCallegari/cibersecurity-desafio-ransomware/blob/main/file-text.jpeg)



2. Arquivo criptografado
   
![imagem de arquivo de texto criptografado](https://github.com/VictorCallegari/cibersecurity-desafio-ransomware/blob/main/encrypt-file.jpeg)

---

## Aviso Legal

Este projeto é **estritamente para fins educacionais** e demonstra o funcionamento básico de criptografia e descriptografia. O uso malicioso deste código é ilegal e altamente desencorajado. O autor não se responsabiliza por qualquer uso indevido.

---

## Autor

Victor Ramos Andrade Callegari


# Aria — IA autoevolutiva (Ahiga Go Life)

A Aria é uma IA em Python que roda no seu computador ou celular. Ela conversa em português e inglês, faz contas, analisa seus dados, estuda temas na internet e evolui sozinha, passando por provas de segurança antes de cada mudança.

## O que ela faz
- **Conversa:** entende frases livres (ex.: "o que é fotossíntese?", "calcule (12+8)*3").
- **Estuda:** `aprenda (tema)` pesquisa no DuckDuckGo e lê **só fontes confiáveis do Brasil** (escolas `.edu.br`, órgãos `.gov.br` e sites educacionais). Sites fora da lista não são abertos.
- **Analisa dados:** média, mediana, desvio e tendência de listas de números e de arquivos `.csv`.
- **Processa fotos:** `/leve foto.png` reduz uma foto pesada; `/pixel foto.png` pega um pixel e a cor exata.
- **Evolui:** cada versão nova passa por 6 pastas de teste (0 teste · 1 ruins · 2 nem · 3 boas · 4 excelentes · 5 perfeitas). Só uma versão melhor assume o lugar da atual.
- **Configurações:** palavras proibidas, sites confiáveis extras, nome da IA, tom, tema e idioma.
- **Arquivos:** envie arquivos pelo 📎 ou arrastando para a janela. A página "Arquivos enviados" mostra o que já foi para a base de dados.

## Como rodar

Você precisa de **Python 3.10 ou mais novo**.

```
pip install flask ddgs deep_translator pillow
python aria.py
```
## DICA: SE NÃO TIVER COM A KEY SEGREDA MUDE O FORMADO DO ARQUIVO aria.txt para .env

Depois abra **http://127.0.0.1:5000**, crie sua conta e converse.

No Termux (Android), o Pillow pode falhar ao compilar. Nesse caso, rode `pkg install python-pillow` antes. Sem o Pillow, a Aria funciona normalmente, só não processa fotos.

## Segurança

- Só as fontes confiáveis são abertas, e redirecionamentos para a rede interna são bloqueados.
- Palavras proibidas bloqueiam a mensagem e são trocadas por `***` nas respostas.
- A IA não executa comandos no seu computador, não apaga arquivos e não altera o próprio código.
- Quando a ajuda coletiva está ligada, um pedaço de foto nunca vai inteiro para outra pessoa, e o servidor confere uma parte das respostas.

"Nenhuma rebelião" nas provas da evolução vale para os testes que a Aria faz. Não é uma garantia absoluta.

## Licença

Projeto sem fins lucrativos.

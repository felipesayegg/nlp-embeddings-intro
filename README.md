# nlp-embeddings-intro

# 🧠 Primeiros Passos em NLP: Tokenização e Word Embeddings

Este projeto é meu **primeiro mergulho prático** no mundo de **Processamento de Linguagem Natural (NLP)**.  
Aqui, eu quis entender **na prática** como modelos como GPT-2 e BERT lidam com texto:  
- Como eles **quebram** uma frase em partes menores (tokens)
- Como transformam essas partes em **números** (IDs)
- E como esses números viram **vetores de significado** (embeddings)

No final, também explorei **como medir a “proximidade”** entre palavras no espaço do modelo usando **similaridade cosseno**.

---

## 🚀 O que eu aprendi e pratiquei

1. **Tokenização com GPT-2**
   - Usei o tokenizador do GPT-2 para ver como ele divide um texto em tokens.
   - Descobri que tokens nem sempre são palavras inteiras — podem ser pedaços!
   - Comparei **quantidade de palavras** vs. **quantidade de tokens**.

2. **Embeddings com BERT (Inglês e Português)**
   - Carreguei o modelo BERT para inglês (`bert-base-uncased`) e para português (`neuralmind/bert-base-portuguese-cased`).
   - Gerei embeddings para tokens e entendi a diferença entre:
     - **Embeddings fixos** (da tabela de vocabulário)
     - **Embeddings contextuais** (que mudam conforme a frase)

3. **Similaridade Cosseno**
   - Comparei pares de palavras como `king` vs `queen`, `cat` vs `dog`, `rei` vs `rainha`.
   - Entendi que valores altos (próximos de 1) significam que o modelo vê as palavras como **semânticamente próximas**.

4. **Diferença entre Modelos**
   - Percebi que cada modelo tem seu **próprio vocabulário** e **tokenização**.
   - Misturar tokenizadores de modelos diferentes causa erro ou resultados falsos.

---

## 📚 Conceitos que ficaram claros para mim

- **Biblioteca, módulo, classe, método**  
  Como importar só o que eu preciso (`from transformers import ...`) e criar objetos a partir de classes usando `.from_pretrained()`.

- **Tokenização**  
  Quebrar texto em partes menores para que o modelo consiga transformar em números.

- **Embeddings**  
  Vetores que representam significado.  
  - Fixos: mesmo vetor sempre para o mesmo token.
  - Contextuais: vetor depende da frase.

- **Similaridade Cosseno**  
  Mede o quanto dois vetores “apontam” para a mesma direção (1 = muito parecidos, 0 = nada a ver).

---

## 🛠 Tecnologias usadas
- [Python 3](https://www.python.org/)
- [Hugging Face Transformers](https://huggingface.co/docs/transformers/index)
- [PyTorch](https://pytorch.org/)

---

## 📂 Estrutura do projeto
- `notebook.ipynb` → código principal (limpo para renderizar no GitHub)
- `aula2_nlp_token_embedding.py` → versão em script
- `requirements.txt` → bibliotecas necessárias

---

## 💡 Próximos passos
- Experimentar embeddings contextuais na comparação de palavras.
- Comparar frases inteiras usando pooling de embeddings.
- Criar visualizações gráficas dos vetores com PCA/t-SNE.

---

✍️ **Autor:** Seu Nome Aqui  
💬 Se quiser trocar ideia sobre NLP ou modelos pré-treinados, é só me chamar!

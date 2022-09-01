## Word2Vec

### what is word2Vec

Word2Vec is one of the [Word Embedding](https://github.com/wlyang538/NLPBasic/blob/main/Word_Embedding.md) methods. it's the process of coverting the words to  calculable and structure vector. 

---

There are two training mode for the Word2Vec.
- CBOW(Continuous Bag-of_words Model)  
- Skip-gram(Continuous Skip-gram Model). 

### CBOW

CBOW use the context to predicate the current word. That means we remove one word from a sentence and let the model guess what the word it is.
For example:
      > Wollongong is a ( output ) city in Australia. 
The output is the word that model need to predict.

### Skip-gram


Skip-gram refers to use the current word to predict the context. That means give you a word, and then the model should predict the words may appear in context.
For example:
      > (output) (output) (output) beautiful (output) (output) (output).
The output is the words that model need to predict.

### The method to optimize

There are two methods we use to speed up the Word2Vec.
- Negative Sample
- Hierarchical Softmax

Google it to see more detail.

### The advantage and disadvantage of Word2Vec

> PS: Word2Vec is the old method that used before 2018, we always use [BERT](https://zhuanlan.zhihu.com/p/46652512) to instead.

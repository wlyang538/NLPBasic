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

#### Advantages:
1. Because the Word2Vec will consider the context. So, compare with the method before, Word2Vec has better effective.
2. Compare with the old method, Word2Vec has low-dimensional vector. that can easy to calulate and store.
3. Can be used in various situations.

#### Disadvantages:
1. Since words and vectors are one-to-one, the problem of polysemy cannot be solved. (由于词和词向量是一对一的关系，所以多义词的问题无法解决。)
2. Word2Vec is a static method. Although it can be used in various situations, it can be optimized Dynamically. (Word2vec 是一种静态的方式，虽然通用性强，但是无法针对特定任务做动态优化
)


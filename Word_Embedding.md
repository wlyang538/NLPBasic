## Word Embedding

### Prepresentation

Text is unstructure information. And this kind of unstructure data cannot be used by NLP model directly. Representation refers to convert the unstructure information into structure information. 

And then, this kind of structure infromation can be calculated by NLP model, and finally can be used to deal with the nlp task.

---

There are three methods for Document representation
- One - hot representation
- Integer encoding （整数编码？）
- word embedding

![image](https://user-images.githubusercontent.com/53561946/187679545-fc477e12-a023-475e-a20c-fa9e5fb1cfa8.png)

#### One-hot Representation

For example, if there are four words in the text, which are dog, cat, cow, and sheep. 
Then, the one-hot representation is:
- cat: [1, 0, 0, 0]
- dog: [0, 1, 0, 0]
- cow: [0, 0, 1, 0]
- sheep: [0, 0, 0, 1]

In the real word, there are lots of different words in corpus. In this situations, the vector will be so long, and most of the element in vector is zero.

So, it may cause some problems. Firstly, it's hard to represent the relationship between words. Secondly, the marix is too sparse, that lead to hard to store and calculate.

#### 整数编码

...Using one number to stand for a word.
For example: cat: 1, dog: 2, cow: 3, sheep:4.

So，this encoding method cannot represent the relationship between words. and Model cannot explain it easily.

#### Word Embedding

Word embedding is the method of text representation. Just like one-hot but have lots of advantages
1. It can use a low-dimentional vector to represent the data
2. It will be very close in space, if they have very similar sematic.
3. It very versatile, and can be used in verial task.

![image](https://user-images.githubusercontent.com/53561946/187730126-9cf6b3d0-c3a8-4b34-b7fe-24a38c1d013c.png)

---

### Word Embedding algorithms

There are two main word embedding algorithms:
- Word2Vec
- GloVe



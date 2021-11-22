# Bengali-Word2Vec-on-Bangla-News-Dataset

<h2 align="left">Info:</h2>
This is a word2vec model created on bengali news dataset.This model can be used in NLP tasks.

Download two other files from this link and put them in same folder:

<li><a href="https://drive.google.com/file/d/1lm6-IDMxfY-_lkIaRxMhanz1tjevKeEQ/view?usp=sharing">First File</a></li></br>
<li><a href="https://drive.google.com/file/d/1LbxhTXmyGTKCiTS2O6EtdbndklSo9WgP/view?usp=sharing">Second File</a></li></br>


<h2 align="left">Installation:</h2>

```python
pip install gensim
```

</br>
<h2 align="left">Training Details:</h2>
<h5 align="left">Number of Sentences: 3248295</h5>
<h5 align="left">Number of Words: 42466428</h5>
<h5 align="left">Number of Unique Words: 461498</h5>
<h5 align="left">Vector Size: 250</h5>

<h2 align="left">Example:</h2>

<h4 align="left">Most Similar Word</h4>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar('লাশ',topn=10))
```

<pre>[('মরদেহ', 0.94624263048172), ('মৃতদেহ', 0.8348001837730408), ('লাশটি', 0.7794113755226135), ('মরদেহটি', 0.7031034827232361), ('মৃতদেহটি', 0.5887435674667358), ('লাশগুলো', 0.585713267326355), ('লাশও', 0.5793684124946594), ('অর্ধগলিত', 0.5611011981964111), ('দেহাবশেষ', 0.5305518507957458), ('শিশুটিকে', 0.5166477560997009)] 
</pre>


```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar('আর্সেনাল',topn=10))
```

<pre>[('লিভারপুল', 0.864025890827179), ('ম্যানইউ', 0.859952449798584), ('জুভেন্টাস', 0.859228789806366), ('চেলসি', 0.857848584651947), ('ম্যানসিটি', 0.8564266562461853), 
('টটেনহ্যাম', 0.8278807401657104), ('বায়ার্ন', 0.8161858916282654), ('আতলেতিকো', 0.8077094554901123), ('পিএসজি', 0.8006083965301514), ('অ্যাটলেটিকো', 0.8002341389656
067)]
</pre>


```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar('বুধবার',topn=10))
```

<pre>[('বৃহস্পতিবার', 0.9739387631416321), ('মঙ্গলবার', 0.9737098217010498), ('সোমবার', 0.9703750610351562), ('শনিবার', 0.9651323556900024), ('রোববার', 0.9642365574836731
), ('শুক্রবার', 0.9547618627548218), ('রবিবার', 0.9407676458358765), ('গতকাল', 0.7294772863388062), ('বৃস্পতিবার', 0.7177606821060181), ('সোমবার', 0.683220982551574
7)]
</pre>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.similar_by_key('শেরপুর',topn=20))
```

<pre>[('বগুড়া', 0.6987679600715637), ('জয়পুরহাট', 0.6914176344871521), ('শেরপুরের', 0.687629759311676), ('নাটোর', 0.6781008839607239), ('নওগাঁ', 0.674379289150238), ('নাল
িতাবাড়ী', 0.6626357436180115), ('জামালপুর', 0.6599703431129456), ('কিশোরগঞ্জ', 0.6550219655036926), ('আক্কেলপুর', 0.6539381146430969), ('চুয়াডাঙ্গা', 0.6507574319839
478), ('মাগুরা', 0.6438732147216797), ('ঝিনাইদহ', 0.6424745917320251), ('চাঁপাইনবাবগঞ্জ', 0.6341075301170349), ('কুড়িগ্রাম', 0.6304787993431091), ('কোটচাঁদপুর', 0.62
9873514175415), ('নকলা', 0.6286910772323608), ('রাজবাড়ী', 0.627704381942749), ('মেহেরপুর', 0.6272647976875305), ('ঠাকুরগাঁও', 0.626388669013977), ('গাইবান্ধা', 0.621
867835521698)]
</pre>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar('ভ্যান'))
```

<pre>[('পিকআপ', 0.7463464736938477), ('মাইক্রোবাস', 0.7289495468139648), ('রিকশা', 0.7281388640403748), ('প্রাইভেটকার', 0.7158138155937195), ('অটোরিকশা', 0.71521860361099
24), ('ইজিবাইক', 0.6967160105705261), ('কাভার্ড', 0.6805071234703064), ('মোটরসাইকেল', 0.6749200820922852), ('ব্যাটারিচালিত', 0.6715964078903198), ('সিএনজি', 0.670970
4399108887)]
</pre>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar_cosmul('নিহত',topn=10))
```

<pre>[('আহত', 0.8362533450126648), ('নিখোঁজ', 0.8162438869476318), ('নিখোঁজ', 0.8142444491386414), ('গুলিবিদ্ধ', 0.8126031756401062), ('দগ্ধ', 0.7997279763221741), ('নিহ
তের', 0.7862117886543274), ('খুন', 0.7741910219192505), ('আরোহী', 0.7703795433044434), ('মৃত্যু', 0.7670021057128906), ('হতাহত', 0.7641921043395996)]
</pre>





<h4 align="left">Cosine Similarity between two sentences:</h4>


```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
text1 = 'শনিবার দুপুরে ঢাকা মেডিকেল কলেজ হাসপাতালের মর্গ থেকে লাশগুলো হস্তান্তর করা হয়'.split()
text2 = 'নারায়ণগঞ্জের রূপগঞ্জে হাসেম ফুড কারখানায় আগুনে পুড়ে নিহত আরও ২১ জনের লাশ স্বজনদের কাছে হস্তান্তর করা হয়েছে'.split()
print(model.wv.n_similarity(ws1=text1,ws2=text2))
```

<pre>0.43630385
</pre>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
text1 = 'নারায়ণগঞ্জের রূপগঞ্জে সজীব গ্রুপের অঙ্গ প্রতিষ্ঠান হাসেম ফুড লিমিটেড নামে একটি কারখানায় ভয়াবহ অগ্নিকাণ্ডে এ পর্যন্ত মোট ৫২ জন নিহত হয়েছেন'.split()
text2 = 'নারায়ণগঞ্জের রূপগঞ্জে সজীব গ্রুপের অঙ্গ প্রতিষ্ঠান হাসেম ফুড লিমিটেড নামে একটি কারখানায় ভয়াবহ অগ্নিকাণ্ডে এ পর্যন্ত মোট ৫২ জন নিহত হয়েছেন'.split()
print(model.wv.n_similarity(ws1=text1,ws2=text2))
```

<pre>1.0
</pre>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
text1 = 'বগুড়ার শেরপুরে মোটরসাইকেলের ধাক্কায় এক নারী নিহত হয়েছেন'.split()
text2 = 'গোপালগঞ্জের কাশিয়ানীতে পিকআপ ভ্যান ও ট্রাকের সংঘর্ষে পিকআপ ভ্যানের চালক নিহত ও পাঁচজন আহত হয়েছেন'.split()
print(model.wv.n_similarity(ws1=text1,ws2=text2))
```

<pre>0.7514724
</pre>

<h4 align="left">Cosine Similarity between two words:</h4>


```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")

print(model.wv.similarity(w1='চট্টগ্রাম',w2='ঢাকা'))
print(model.wv.similarity(w1='উপজেলা',w2='জেলা'))
print(model.wv.similarity(w1='চাপায়',w2='সেতু'))
print(model.wv.similarity(w1='বুধবার',w2='বুধবার'))
```

<pre>0.6105419
0.5725356
0.08221294
1.0
</pre>

<h4 align="left">Distance between two words:</h4>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.distance('বিদেশি','বাংলাদেশী'))
print(model.wv.distance('দুর্ঘটনা','নিহত'))
```

<pre>0.7254734635353088
0.8778904378414154
</pre>


<h4 align="left">Word Mover's distance between two sentences:</h4>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
text1 = 'বগুড়ার শেরপুরে মোটরসাইকেলের ধাক্কায় এক নারী নিহত হয়েছেন'
text2 = 'গোপালগঞ্জের কাশিয়ানীতে পিকআপ ভ্যান ও ট্রাকের সংঘর্ষে পিকআপ ভ্যানের চালক নিহত ও পাঁচজন আহত হয়েছেন'
print(model.wv.wmdistance(text1,text2))
```

<pre>0.42776958178441427
</pre>

<h4 align="left">Most Similar word from a list of given words:</h4>

```python
import gensim
model = gensim.models.Word2Vec.load("word2vec2.model")
print(model.wv.most_similar_to_given('বগুড়া',['গোপালগঞ্জ','নারী','ভ্যান','পিকআপ','চালক', 'নিহত', 'ও', 'পাঁচজন', 'আহত', 'হয়েছেন']))
```

<pre>গোপালগঞ্জ
</pre>


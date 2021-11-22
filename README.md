# Bengali-Word2Vec-on-Bangla-News-Dataset

<h3 align="left">Info:</h3>
This is a word2vec model created on bengali news dataset.This model can be used in NLP tasks.

Download two other files from this link and put them in same folder:

<li><a href="https://drive.google.com/file/d/1lm6-IDMxfY-_lkIaRxMhanz1tjevKeEQ/view?usp=sharing">First File</a></li></br>
<li><a href="https://drive.google.com/file/d/1LbxhTXmyGTKCiTS2O6EtdbndklSo9WgP/view?usp=sharing">Second File</a></li></br>


<h3 align="left">Installation:</h3>

```python
pip install gensim
```

</br>
<h3 align="left">Training Details:</h3>
<h6 align="left">Number of Sentences: 3248295</h6>
<h6 align="left">Number of Words: 42466428</h6>
<h6 align="left">Number of Unique Words: 461498</h6>

<h3 align="left">Example:</h3>

<h6 align="left">Most Similar Word</h6>

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
print(model.wv.similar_by_key('শেরপুর',topn=20))
```

<pre>[('বগুড়া', 0.6987679600715637), ('জয়পুরহাট', 0.6914176344871521), ('শেরপুরের', 0.687629759311676), ('নাটোর', 0.6781008839607239), ('নওগাঁ', 0.674379289150238), ('নাল
িতাবাড়ী', 0.6626357436180115), ('জামালপুর', 0.6599703431129456), ('কিশোরগঞ্জ', 0.6550219655036926), ('আক্কেলপুর', 0.6539381146430969), ('চুয়াডাঙ্গা', 0.6507574319839
478), ('মাগুরা', 0.6438732147216797), ('ঝিনাইদহ', 0.6424745917320251), ('চাঁপাইনবাবগঞ্জ', 0.6341075301170349), ('কুড়িগ্রাম', 0.6304787993431091), ('কোটচাঁদপুর', 0.62
9873514175415), ('নকলা', 0.6286910772323608), ('রাজবাড়ী', 0.627704381942749), ('মেহেরপুর', 0.6272647976875305), ('ঠাকুরগাঁও', 0.626388669013977), ('গাইবান্ধা', 0.621
867835521698)]
</pre>




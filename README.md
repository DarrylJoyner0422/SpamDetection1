<h1>Classification and Evaluation to Detect Spam</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
<br />

In this project I will build classification models and calculate metrics for their performance. 

The scenario I will address is "spam" e-mail detection. This is a very important and widely-used supervised machine learning task that attempts to find unsolicited, mass-produced messages that have irrelevant and/or inappropriate content (often mass marketing or attempts at fraud). These are sometimes called "spam filters".

I will treat this task as a binary classification problem: detecting if an email is "spam" (Class == 1) or not (Class == 0, a regular/good e-mail). Email systems will typically automatically move messages detected as "spam" to a "Spam" or "Deleted" folder so the user will not have to read them in their regular inbox.

In this setup, a false positive would mark a regular/good e-mail as spam. The key aspect of the "spam" scenario is that false positives are obviously very undesirable, because these would cause people to potentially lose valuable "good" messages. So I will aim for a highly precise spam filter that has few/no false positives. As a consequence it may let more spam through the filter. This is a classic precision / recall tradeoff, which I will explore and  investigate.



<h2>Python Libraries Used</h2>

- <b>Matplotlib (matplotlib.pyplot): For plotting and data visualization.</b> 
- <b>Pandas (pandas): For data manipulation and analysis.</b>
- <b>Seaborn (seaborn): For statistical data visualization</b>
- <b>Scikit-learn (sklearn):</b>
- <b>TfidfVectorizer: For converting text data into TF-IDF feature vectors.</b>
- <b>ENGLISH_STOP_WORDS: A set of common English stop words.</b>
- <b>LogisticRegression: For building a logistic regression classifier.</b>
- <b>f1_score: For evaluating the classifier using the F1 score.</b>
- <b>make_pipeline: For creating a machine learning pipeline.</b>
- <b>tqdm: For displaying progress bars.</b>



<h2>Environments Used </h2>

- <b>Jupyter</b> (21H2)



<h2>Program walk-through:</h2>

<p align="left">








---------------------------Start New ------------------------------------------



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>








<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
















<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>





<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>






<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>












<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>














<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>















<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>













<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
















<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>






<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>






<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>












<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>














<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>















<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>













<br />
<br />
NEXT PICTURE:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>











-------------------------------------End New--------------------------------------------



</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

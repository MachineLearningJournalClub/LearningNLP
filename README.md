<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="https://github.com/MachineLearningJournalClub/LearningNLP">
    <img src="img/logos/logo_mljc.png" alt="Logo" width="120" height="120">
  </a>

  <h1 align="center">Learning NLP</h1>
  <h3 align="center">Some Tutorials and in depth analysis of Natural Language Processing (NLP) techniques and applied NLP</h3>

  <p align="center">
    <br />
    <a href="https://github.com/MachineLearningJournalClub/LearningNLP"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/MachineLearningJournalClub/LearningNLP">View Demo</a>
    ·
    <a href="https://github.com/MachineLearningJournalClub/LearningNLP/issues">Report Bug</a>
    ·
    <a href="https://github.com/MachineLearningJournalClub/LearningNLP/pulls">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>  
        <li><a href="#tutorial-1">Tutorial 1</a></li>
        <li><a href="#tutorial-2">Tutorial 2</a></li>
        <li><a href="#tutorial-3">Tutorial 3</a></li>
        <li><a href="#tutorial-4">Tutorial 4</a></li>
      </ul>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

ADD PROJECT DESCRIPTION + TWO LINES ABOUT MLJC

### Built With

* []()
* []()
* []()



<!-- GETTING STARTED -->
# Getting Started

You can either get a local copy by downloading this repo or either use [Google Colaboratory](https://colab.research.google.com/) by copy-pasting the link of the notebook (.ipynb file) of your choice.


### Prerequisites 

**Install Miniconda (Local Version)**

Please go to the [Anaconda website](https://conda.io/miniconda.html).
Download and install *the latest* Miniconda version for *Python* 3.8 for your operating system.

```bash
wget <http:// link to miniconda>
sh <miniconda*.sh>
```

**Download This Repo (Local Version)**
```bash
git clone https://github.com/MachineLearningJournalClub/LearningNLP
```

**Setup Conda Environment (Local Version)**
IN THE END WE CAN SETUP A CONDA ENVIRONMENT AND EXPORT REQUIREMENTS (NEEDED LIBRARIES)

Change directory (`cd`) into the LearningNLP folder, then type:

```bash
# cd LearningNLP
conda env create -f environment.yml
source activate LNLP
```

-------
## [Tutorial 1](https://github.com/MachineLearningJournalClub/LearningNLP/blob/main/LearningNLP_Tutorial1.ipynb)

### Topics 
* Sentiment Analysis with Logistic Regression 
* Sentiment Analysis with Naive Bayes 
* Word Vectorizing (CountVectorizer in Scikit-learn)
* Some Explainability Methods

### Notebook 

* Dataset: [ArXiv from Kaggle](https://www.kaggle.com/Cornell-University/arxiv)
* Preprocessing: [pandas](https://pandas.pydata.org/docs/), [nltk](https://www.nltk.org/), [gensim](https://radimrehurek.com/gensim/) 
* Binary classification: Scikit-learn's [CountVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html) + [TfidfTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfTransformer.html?highlight=tfidf#sklearn.feature_extraction.text.TfidfTransformer) 
* Explainability Methods: [LIME](https://christophm.github.io/interpretable-ml-book/lime.html#lime), [SHAP](https://christophm.github.io/interpretable-ml-book/shap.html)

  Useful references for explainibility methods: 
  * LIME, [Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938) 
  * SHAP, [A Unified Approach to Interpreting Model Predictions](https://arxiv.org/abs/1705.07874v2)
  * Adversarial attacks (have you heard of?), i.e. how to fool algorithms --> [Fooling LIME and SHAP: Adversarial Attacks on Post hoc Explanation Methods](https://arxiv.org/abs/1911.02508)
  
* Open Questions for you: 
  * How to deal with multiclass problems? 
  * Try to develop binary classification with abstracts instead of titles
  * Try to develop the same pipeline with [spaCy](https://spacy.io/)

-------
## [Tutorial 2](https://github.com/MachineLearningJournalClub/LearningNLP/blob/main/LearningNLP_Tutorial2.ipynb)


### Topics 

* Bias & Fairness in NLP (Ethics and Machine Learning)
* Gender Framing (in Political Tweets)
* Political Party Prediction
* Topic Modeling - Latent Dirichlet Allocation (LDA)

### [Slides](https://github.com/MachineLearningJournalClub/LearningNLP/blob/main/LearningNLP_Slides_Tutorial2.pdf)

We'd like to introduce some ethical concerns in ML and especially in NLP, the idea is to start a long-term project directed towards Bias & Fairness in Machine Learning, i.e. intrinsic problems in our data can create inequalities in the real world (Have you watched *"Coded Bias"* on Netflix?)

### Notebook 

* Dataset: we created [a dataset](https://www.kaggle.com/marinar/tweets-some-of-house-of-representative) by scraping tweets from some US politicians 
* Preprocessing: [pandas](https://pandas.pydata.org/docs/), [nltk](https://www.nltk.org/), [gensim](https://radimrehurek.com/gensim/) 
* Binary classification: Scikit-learn's [CountVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html) + [TfidfTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfTransformer.html?highlight=tfidf#sklearn.feature_extraction.text.TfidfTransformer) 
* Topic Modeling by employing [Latent Dirichlet Allocation ](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation)(LDA) + visualization. Some educational contents for LDA: [L. Serrano part 1 on LDA](https://www.youtube.com/watch?v=T05t-SqKArY), [L. Serrano part 2 How to train LDA](https://www.youtube.com/watch?v=BaM1uiCpj_E)

   

-------
## Tutorial 3

### Topics 

* Global Vectors for word representations (GloVe), [Stanford NLP](https://nlp.stanford.edu/pubs/glove.pdf)
* [Fasttext](https://fasttext.cc/docs/en/unsupervised-tutorial.html), skipgrams vs CBOWs
* Bias in Word Embeddings (Gender + Ethnic Stereotypes) 


### Possible Ideas: 

* Word embeddings quantify 100 years of gender and ethnic stereotypes, [PNAS paper](https://www.pnas.org/content/pnas/115/16/E3635.full.pdf) + [code](https://github.com/nikhgarg/EmbeddingDynamicStereotypes)
* Understanding Bias in Word Embeddings, [ICML paper](http://proceedings.mlr.press/v97/brunet19a.html) + [code](https://github.com/mebrunet/understanding-bias)

-------
## Tutorial 4

### Topics 
* Autocomplete and Language Models
* Word embeddings with neural networks

### Possible Ideas: 

------

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/MachineLearningJournalClub/LearningNLP/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Marina Rizzi - email : []() - [linkedin]()

Alessio Borriero - email : [alessio.borriero@edu.unito.it](alessio.borriero@edu.unito.it) - [linkedin](https://www.linkedin.com/in/alessio-borriero-357724183/)

Simone Azeglio - email : [simone.azeglio@edu.unito.it](simone.azeglio@edu.unito.it) - [linkedin](https://www.linkedin.com/in/simoneazeglio/)

Micol Olocco - email : []() - [linkedin]()

Luca Bottero  - email : []() - [linkedin]()


Project Link: [https://github.com/MachineLearningJournalClub/LearningNLP](https://github.com/MachineLearningJournalClub/LearningNLP)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

<p align="center">
   <a href="https://github.com/MachineLearningJournalClub/LearningNLP">
    <img src="img/logos/logo_hpc4ai.png" alt="Logo" width="300" height="120">
    
  </a>

* [HPC4AI](https://hpc4ai.it/)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/MachineLearningJournalClub/LearningNLP.svg?style=for-the-badge
[contributors-url]: https://github.com/MachineLearningJournalClub/LearningNLP/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/MachineLearningJournalClub/LearningNLP.svg?style=for-the-badge
[forks-url]: https://github.com/MachineLearningJournalClub/LearningNLP/network/members
[stars-shield]: https://img.shields.io/github/stars/MachineLearningJournalClub/LearningNLP.svg?style=for-the-badge
[stars-url]: https://github.com/MachineLearningJournalClub/LearningNLP/stargazers
[issues-shield]: https://img.shields.io/github/issues/MachineLearningJournalClub/LearningNLP.svg?style=for-the-badge
[issues-url]: https://github.com/MachineLearningJournalClub/LearningNLPissues
[license-shield]: https://img.shields.io/github/license/MachineLearningJournalClub/LearningNLP.svg?style=for-the-badge
[license-url]: https://github.com/MachineLearningJournalClub/LearningNLP/blob/main/LICENSE.md
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/company/machine-learning-journal-club




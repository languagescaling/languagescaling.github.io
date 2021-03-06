<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.3/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
    MathJax.Hub.Config({
        extensions: ["tex2jax.js"],
        jax: ["input/TeX", "output/HTML-CSS"],
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
        },
        "HTML-CSS": { availableFonts: ["TeX"] }
    });
</script>

## Abstract

Natural Language Processing models have achieved impressive performance, thanks to the recent deep learning approaches. However, large deep learning models typically rely on huge amounts of human labeled data. There are more than [7,000 languages](https://www.ethnologue.com/) spoken in the world. Unfortunately, most languages have very limited linguistic resources. Language scaling is invaluable to the advance of social welfare, and thus has attracted intensive interest from industrial practitioners who want to deploy their applications/services to global markets. At the same time, due to the huge differences in the vocabulary, morphology and syntax among different languages, scaling out NLP applications to various languages presents grand challenges to machine learning, data mining, and natural language processing.


In this tutorial, we systematically survey the frontier of language scaling using as examples the research, techniques, and engineering behind a series of concrete NLP applications in Microsoft products and services that need to be scaled out to 100+ languages. We start with a clear problem description for language scaling and an intuitive discussion on the overall challenges,. Then, we explore the problem from data perspective, including the availability of different types of training data as well as the evaluation benchmark data sets for various tasks. A large part of the tutorial will focus on various approaches to language scaling, including cross-lingual models, data augmentation, and language knowledge transferring algorithms. We have applied different approaches for various applications and built a platform to integrate our approaches. Using this platform we will demonstrate several case studies that have been shipped to Microsoft products, and share with the audience our lessons and experience learned. Finally, we will discuss several important challenges in this area and future directions.

## Tutorial Materials 
- [Introduction](https://github.com/languagescaling/languagescaling.github.io/blob/main/TheWebConf'21_Tutorial_Scaling_out_NLP_Applications_to_100__Languages.pdf)
- [Tutorial Slides](https://github.com/languagescaling/languagescaling.github.io/blob/main/Scaling-out-NLP-applications-to-100%2B-languages-slides.pdf)
- [Tutorial Video](https://www.youtube.com/watch?v=K7nDlS4r7tg)

## Presenters

### Daxin Jiang ([homepage](https://www.microsoft.com/en-us/research/people/djiang/))

<img src="./figures/daxin.jpg" align="left" width="15%" hspace="10" vspace="1">**Daxin Jiang, Ph.D., Chief Scientist, Microsoft Software Technology Center Asia.** Daxin Jiang has years of experience of Research and Engineering in Machine Learning, Data Mining, Natural Language Processing, and Bioinformatics. He received Ph.D. in Computer Science from the Statue University of New York at Buffalo in 2005. He has published extensively in prestigious conferences and journals, and served as a PC member of numerous conferences. He received Best Application Paper Award of SIGKDD'08 and Runner-up for Best Application Paper Award of SIGKDD'04. Daxin is leading an R\&D group in Microsoft with 170+ applied scientists and engineers to develop NLP algorithms, applications and platforms, which support various Microsoft products, including Bing, Cortana, Teams, Outlook, and Microsoft Cognitive Services.

Address: 5 Danling Street, Hai Dian, Beijing, China, 100080.  Email: djiang@microsoft.com. Tel: +86 (10) 5917 3321.

### Jian Pei ([homepage](https://www.cs.sfu.ca/~jpei/))

<img src="./figures/jianpei.jpg" align="left" width="15%" hspace="10" vspace="1">**Jian Pei, Ph.D., Professor, School of Computing Science, Simon Fraser University.** His expertise is in developing effective and efficient data analysis techniques for novel data intensive applications. He is a research leader in the general areas of data science, big data, data mining, and database systems. He is recognized as a fellow of Royal Society of Canada (RSC) (i.e., the national academy of Canada), the Canadian Academy of Engineering (CAE), ACM and IEEE. He is one of the most cited authors in data mining, database systems, and information retrieval. His research has generated remarkable impact substantially beyond academia. His algorithms have been adopted by industry in production and popular open source software suites. He is responsible for several commercial systems of record-breaking large scale. As a renowned professional leader, he has played important roles in many academic organizations and activities. He is the Chair of ACM SIGKDD and was the Editor-in-Chief of IEEE TKDE. He received many prestigious awards, including the 2017 ACM SIGKDD Innovation Award and the 2015 ACM SIGKDD Service Award. In his last leave-of-absence from the university, he took the executive roles of two Fortune Global 500 companies. He is a mentor of Creative Destruction Lab (CDL).

Address: 8888 University Drive, Burnaby, BC Canada, V5A 1S6. Email: jpei@cs.sfu.ca. Tel: +1 (778) 782 6851. Fax: +1 (778) 782 3045.

### Linjun Shou ([homepage](https://www.microsoft.com/en-us/research/people/lisho/))

<img src="./figures/lisho-me.jpg" align="left" width="15%" hspace="10" vspace="1"> **Linjun Shou, Senior Applied Scientist Manager, Microsoft Software Technology Center Asia.** He has good publications on several prestigious international conferences such as ACL, EMNLP, COLING, SIGKDD, AAAI, WSDM, etc and served as the program committees on numerous conferences. His research interests include question answering, cross lingual transfer learning, representation learning, etc. Plenty of his research has been transferred to real Microsoft products such as Bing universal question answering, query understanding, document understanding, news/tweets ranking systems. Besides, he is also actively contributing to the academic community through open sourcing projects (e.g. [NeuronBlocks](https://github.com/microsoft/NeuronBlocks)) and benchmarks like [XGLUE](https://github.com/microsoft/XGLUE), [CodeXGLUE](https://github.com/microsoft/CodeXGLUE).

Address: 5 Danling Street, Hai Dian, Beijing, China, 100080.  Email: lisho@microsoft.com. 

### Ming Gong ([homepage](https://www.microsoft.com/en-us/research/people/migon/))

<img src="./figures/Ming-Photoes.jpg" align="left" width="15%" hspace="10" vspace="1"> **Ming Gong, Ph.D., Principal Applied Scientist Manager, Microsoft Software Technology Center Asia.** She received Ph.D. on Graphics and Visual Computing in 2013 from Institute of Computing Technology, Chinese Academy of Sciences. She is leading an elite team with 10+ applied scientists and engineers to develop novel NLP technologies for AI applications. Her research interests include question answering, search intelligence, multilingual/cross-modal modeling, representation learning, etc. She published 30+ papers in top conferences and journals (e.g. ACL, COLING, SIGKDD, EMNLP, WSDM, AAAI, PR, CVIU), and also served as PC members of top NLP/AI conferences. Besides, she is actively contributing to the academic community by open-sourcing projects (e.g. [NeuronBlocks](https://github.com/microsoft/NeuronBlocks))  and benchmarks like [XGLUE](https://github.com/microsoft/XGLUE), [CodeXGLUE](https://github.com/microsoft/CodeXGLUE).  Many of the novel technologies have been transferred to Microsoft’s global products and online services including Bing search, multilingual question answering services and document understanding platform. 

Address: 5 Danling Street, Hai Dian, Beijing, China, 100080.  Email: migon@microsoft.com.

### Xiubo Geng ([homepage](https://xiubo0211.github.io/))

<img src="./figures/xiubo-photo.png" align="left" width="15%" hspace="10" vspace="1"> **Xiubo Geng, Ph.D., Senior Applied Scientist, Microsoft Software Technology Center Asia.** She received Ph.D in Computer Science in 2011 from Institute of Computing Technology, Chinese Academy of Sciences. Her research interests include machine learning, search intelligence, question answering, multilingual modeling, reasoning, etc. She has good publications on top conferences (e.g. SIGIR, NeurIPS, WWW, EMNLP, IJCAI, etc.), and served as a PC member of several conferences.

Address: 5 Danling Street, Hai Dian, Beijing, China, 100080.  Email: xigeng@microsoft.com.

### Xinjie Zhou

<img src="./figures/xinjie.jpg" align="left" width="15%" hspace="10" vspace="1"> **Xinjie Zhou, Ph.D., Senior Software Engineer Lead, Microsoft Software Technology Center Asia.** He received Ph.D. on natural language processing in 2017 from Peking University. His research interests include machine learning, natural language understanding, multilingual modeling, etc. He has good publications on top conferences including ACL, EMNLP, AAAI, etc.

Address: Bldg \#25, 328 Xinghu Street, SIP, Suzhou, China, 215000.  Email: xinjzhou@microsoft.com.



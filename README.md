<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']],
            displayMath: [ ['$$','$$']],
            }
        });
    </script>
</head>

## Authors

>$$\texttt{Linjun Shou}^{\dagger}, \texttt{Ming Gong}^{\dagger}, \texttt{Jian Pei}^{\ddagger}, \texttt{Xiubo Geng}^{\dagger}, \texttt{Xingjie Zhou}^{\dagger} \texttt{and } \texttt{Daxin Jiang}^{\dagger}$$

>$${ }^\dagger\texttt{Microsoft STCA NLP Group, Beijing, China}$$
>$${ }^\ddagger\texttt{School of Computer Science, Simon Fraser University}$$
>$$\texttt{lisho, migon, xigeng, xingzhou, djiang\}@microsoft.com\ jpei@cs.sfu.ca}$$


## Abstract

Natural Language Processing models have achieved impressive performance, thanks to the recent deep learning approaches. However, large deep learning models typically rely on huge amounts of human labeled data. There are more than [7,000 languages](https://www.ethnologue.com/) spoken in the world. Unfortunately, most languages have very limited linguistic resources. Language scaling is invaluable to the advance of social welfare, and thus has attracted intensive interest from industrial practitioners who want to deploy their applications/services to global markets. At the same time, due to the huge differences in the vocabulary, morphology and syntax among different languages, scaling out NLP applications to various languages presents grand challenges to machine learning, data mining, and natural language processing.


In this tutorial, we systematically survey the frontier of language scaling using as examples the research, techniques, and engineering behind a series of concrete NLP applications in Microsoft products and services that need to be scaled out to 100+ languages. We start with a clear problem description for language scaling and an intuitive discussion on the overall challenges,. Then, we explore the problem from data perspective, including the availability of different types of training data as well as the evaluation benchmark data sets for various tasks. A large part of the tutorial will focus on various approaches to language scaling, including cross-lingual models, data augmentation, and language knowledge transferring algorithms. We have applied different approaches for various applications and built a platform to integrate our approaches. Using this platform we will demonstrate several case studies that have been shipped to Microsoft products, and share with the audience our lessons and experience learned. Finally, we will discuss several important challenges in this area and future directions.









<center class="half">
    <img src="./figures/ms.png" height="150" width="300"/> 
    <img src="./figures/sfu.png" height="150"  width="300"/>
</center>


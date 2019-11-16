# Texture

- [mitの講義資料集](http://cvcl.mit.edu/sunslides/)
  - textureについてのスライドがある．

- [Barkeleyの講義資料集](https://people.eecs.berkeley.edu/~trevor/CS280Notes/?C=N;O=A)

- [Pyramid-Based Texture Analysis/Synthesis](https://www.cns.nyu.edu/heegerlab/content/publications/Heeger-siggraph95.pdf) 
  - steerable pyramidを用いて，ヒストグラムマッチングという手法を用いて，texture合成を行っている．

    - 参考文献 
Our approach is motivated by research on human texture perception.
Current theories of texture discrimination are based on the fact that
two textures are often difficult to discriminate when they produce
a similar distribution of responses in a bank of (orientation and
spatial-frequency selective) linear filters
私たちのアプローチは、人間の質感知覚に関する研究によって動機付けられています。
テクスチャ識別の現在の理論は、2つのテクスチャが（方向および空間周波数選択性）線形フィルタのバンクで応答の同様の分布を生成する場合、識別が難しいことが多いという事実に基づいています[2、3、7、16、20 、32]。したがって、ここで説明する方法は、フィルター出力の分布（またはヒストグラム）を一致させることでテクスチャを合成します。このアプローチは、テクスチャ画像を特徴付けるすべての空間情報を、適切に選択された線形フィルタ出力のセットの1次統計でキャプチャできるという原則に基づいています（これは完全に正しいわけではありません）。それでも、このモデルは（不完全ではありますが）テクスチャプロパティの興味深いセットをキャプチャします。

  - 3.[Early Vision and Texture Perception](http://invibe.net/biblio_database_dyva/woda/data/att/b56c.file.pdf)
  - 7.[Orthogonal Distribution Analysis: A New Approach to the Study of Texture Perception.](https://psycnet.apa.org/record/1991-98916-019)
  - 16.[Texture Segregation and Orientation Gradient.](https://www.cns.nyu.edu/~msl/papers/landybergen91.pdf)
  - 20 .[Preattentive Texture Discrimination with Early Vision Mechanisms](https://pdfs.semanticscholar.org/d31b/ec7d4dcf257c2b24189005dcb441d707d9c2.pdf)
  - 32.[Texture discrimination by Gabor functions](https://link.springer.com/article/10.1007/BF00341922)
  - [Visual Perception of Texture](https://www.researchgate.net/publication/2385560_Visual_Perception_of_Texture)
- [The Heeger-Bergen Pyramid-Based Texture Synthesis Algorithm](https://www.ipol.im/pub/art/2014/79/)
  - 上の論文のアルゴリズムを明確に示している．
- [A parametric Texture Model Based on Joint Statistics of Complex Wavelet Coefficients](https://www.researchgate.net/publication/2441269_A_Parametric_Texture_Model_Based_on_Joint_Statistics_of_Complex_Wavelet_Coefficients)
  - [python実装ブログ](https://www.eranger.co.jp/blog/advanced-technology/%E3%80%90ai%E3%82%A2%E3%83%BC%E3%83%88%E3%80%91portilla%E3%81%A8simoncelli%E3%81%AE%E3%83%86%E3%82%AF%E3%82%B9%E3%83%81%E3%83%A3%E5%90%88%E6%88%90-a-parametric-texture-model-based-on-joint-statistics)

- [The steerable pyramid: A flexible architecture for multi-scale derivative computation](https://www.researchgate.net/publication/3666212_The_steerable_pyramid_A_flexible_architecture_for_multi-scale_derivative_computation)

- [Simoncelliさんのスライド](https://ocw.mit.edu/resources/res-9-003-brains-minds-and-machines-summer-course-summer-2015/unit-4.-visual-intelligence/MITRES_9_003SUM15_sem4-1.pdf)
  - おもしろそう

- [Metamers of the ventral stream](http://www.cnbc.cmu.edu/~tai/cp_papers/metamer_nn.2889.pdf)
  - 周辺視野における知覚全般に当てはまることが指摘されている．(by 21\_304.pdf)

- [Image Style Transfer Using Convolutional Neural Networts](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)
  - コスト関数を論文同様に正規化して実装した．[git](https://github.com/yusuke0055/neural-style-transfer)
- [Texture Synthesis Using Convolutional Neural Networks](https://papers.nips.cc/paper/5633-texture-synthesis-using-convolutional-neural-networks.pdf)
  - スタイルロスのみを用いてtexture合成をした
- [Controlling perceptual factors in neural style transfer](http://openaccess.thecvf.com/content_cvpr_2017/html/Gatys_Controlling_Perceptual_Factors_CVPR_2017_paper.html)
  - 本家著者の論文
- [A parametric texture model based on deep convolutional features closely matches texture 
appearance for humans](https://jov.arvojournals.org/article.aspx?articleid=2657215)
  - Style Transferの著者もいる．style transferのstyle loss + power spectrumを導入してるぽい．
PSS + Style Transfer
- [Deep Correlations for Texture Synthesis](https://dl.acm.org/citation.cfm?id=3015461)

 - [Perceptual Losses for Real-Time Style Transfer and Super-Resolution](https://cs.stanford.edu/people/jcjohns/papers/eccv16/JohnsonECCV16.pdf)
  - Style Transferを高速化しただけ．
- [Stable and Controllable Neural Texture Synthesis and Style Transfer Using Histgram Losses](https://arxiv.org/pdf/1701.08893.pdf)
  - 名前的にヒストグラムマッチング導入してそう．
- [High-Resolution Multi-Scale Neural Texture Synthesis](https://wxs.ca/research/multiscale-neural-synthesis/)
  - StyleLossにmulti-scale Gaussian Pyramidを用いている．素直だと思う．
  - [日本語の解説記事](https://qiita.com/dsanno/items/97eb3a28f3614407a5c4)

- [Texture Synthesis by Non-parametric Sampling](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/papers/efros-iccv99.pdf)



# CNN
- [Deep convolutional networks do not classify based on global object shape](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006613#sec001) 
  - 大域的な特徴をCNNは見ていないって話．
  - [記事](https://ai-scholar.tech/others/cnn-shap-ai-110/)

- [Adversarial Examples Are Not Bugs, They Are Features](http://gradientscience.org/adv/)
  - 

- [Style transferをResnet50でやってみた話．下の記事同様うまくいってない](https://github.com/Leo8216/Neural-Style-Transfer-using-ResNet50-with-tf.keras-)
  - style transferは捉えてる特徴をみるツールになりうる．

- [Neural Style Transfer with Adversarially Robust Classifiers](https://reiinakano.com/2019/06/21/robust-neural-style-transfer.html)
  - [この人のtwitter](https://twitter.com/reiinakano)
 
-  [The Unreasonable Effectiveness of Deep Features as a Perceptual Metric](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zhang_The_Unreasonable_Effectiveness_CVPR_2018_paper.pdf)

- [What do Deep Networks Like to See?]
(http://openaccess.thecvf.com/content_cvpr_2018/papers/Palacio_What_Do_Deep_CVPR_2018_paper.pdf)

# Memo
- dVgg/dPss的なやつをみる
- 

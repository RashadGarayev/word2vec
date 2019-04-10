# word2vec

----------

# Natural Language Processing(NLP) #

T?snifat?na gor? dill?ri iki qrupa bols?k:
> T?bii dill?r 
v? Sunii dill?r

Gund?lik h?yat?m?zda istifad? etdiyimiz dill?r(Ingilis,Ispan,Az?rbaycan,Rus dill?ri) t?bii dil olaraq adlan?r.Bir-birimiz? fikrimizi dil vasit?sil? catd?r?r?q.Suni dill?r? misal olaraq Turing mas?nlar? uz?rind? cal?san xususi dill?rdir(0 v? 1,Pascal,Fortan,C/C++,Python,Java v? s).B?hs etdiyimiz "t?bii dil isl?m?(NLP)" bir dild?ki cuml?ni oxumas? v? basqa bir dild? uygun bir cuml?y? uygunlugunun t?skili mas?n cevirm?l?ridir.NLP -nin cal?sma prinspi,t?bii bir dil uz?rind?-daxilind? ifad? olunan h?r bir k?lim?-xarakterl?rd?n v? ya bayt array-d?n t?skil olunan modell?rdir([https://www.deeplearningbook.org/](https://www.deeplearningbook.org/ "Deep Learning book"))
> Bir dil modeli,t?bii dild? token vektoru uz?rind? t?xmini dag?l?m t?yin edir.Modelin haz?rlanmas?na bagl? olaraq,tokenl?r - bir k?lim?,xarakter v? ya bayt ola bilirl?r.Ilk olaraq dil modell?ri n-gram adland?r?lan sabit uzunluqdak? token vektorlar?n?n modell?rind?n t?skil olunmusdur(Bundan basqa skip-gram,cbow).

----------
> 
Ifad?l?ri r?q?msal ifad? etdiyimiz zaman h?min k?lim?l?r uz?rind? riyazi ?m?liyyatlar aparmaq daha ## rahatd?r.
H?r bir ifad?ni one-hot vektor olaraq t?svir ets?k 

<p align="center"> <img src="image/one-hot.jpg" alt="drawing" width="500"/> </p>


Yuxar?dak? r?simd? gost?ril?n ilk F?ls?f? ifad?si vektor olaraq uygunluq indeksi -0,
 Insan k?lim?si vektor daxilind? birinci indeksd? dayan?r.

Yuxar?dak? t?svir? ?saslansaq,ifad? say? coxald?qca k?lim?l?ri tan?mlamaq c?tinl?s?c?q.Bunun ucun alternativ olaraq one-hot vektoru deyil,h?r bir k?lim?ni vektor il? t?skil edib(word2vec) h?r bir vektor k?lim? ucun 0 v? 1 aras?nda h?qiqi ?d?d tipind? gost?r?c?yik.

Embedding Matrix(word vector,word embedding)

> Insan([ 3.26409712e-02, -1.11495465e-01, -1.09878801e-01, -1.61514040e-02,
        6.24946095e-02, -5.53264767e-02,  1.88343860e-02, -3.00338143e-03,
       -1.54164627e-01, -6.94016367e-02,  1.75558016e-01,  8.69417936e-02..................] size=200


>F?ls?f? ([ 0.03672487, -0.11063578, -0.09298438, -0.01961881,  0.05883814,
       -0.05005358,  0.01460049, -0.00244978, -0.15134725, -0.07507091,
        0.1764792 ,  0.08856005, -0.11544561,  0.13122901,  0.02955697,
       -0.08000021, -0.10689594,  0.00531672, -0.07659401, -0.01527801,
       -0.27507988,  0.04865298,  0.01300979, -0.1417728 , -0.03595459.........................] size=200


----------

Vektorlar? t?skil etm?k ,ucun cuml? daxilind? secil?n soz(ifad?) ?traf?ndak? sozl?rl? ?laq?sini t?yin ed?r?k haz?rlayacag?q.(Qeyd edimki sag v? sol k?lim? uygunlugunu t?sadufi deyil,window-parametri il? biz secirik)
<p align="center"> <img src="image/v.jpg" alt="drawing" width="400"/> </p>

# Korpusun haz?rlan?lmas? #
Az sayda k?lim?l?rd?n t?skil olun korpus,biz? ist?diyimiz modelin n?tic?sini verm?y?c?k.Bunun ucun daha prespektiv wiki layih?l?ri kimi k?lim?l?r toplusu olan datalara ehtiyyac?m?z var.Yuxar?da qeyd olunan korpus sad?c? numun? ucun haz?rlan?lm?sd?r.N?tic? etibar? il? k?lim?y? ?n yax?n dig?r k?lim?l?rin bir nec?si uygunluq t?skil etmisdir.

word2vec vasit?sil? k?lim? vektoru haz?rlamaq  ucun iki f?rqli alqoritmd?n istifad? olunur
> skip-gram
> cbow alqoritmas?

Istifad? etdiyimiz kodlarda skip-gram alqoritmas?na n?z?r yetir?k.(Qeyd vektorlar?n haz?rlan?lmas?nda alqoritman? qeyd etm?s?niz normal halda cbow-alqrt ?lav? olunur-DEFAULT:CBOW)

<p align="center"> <img src="image/skipg.jpg" alt="drawing" width="500"/> </p>

----------
`$ git clone https://github.com/RashadGarayev/word2vec`

`$ cd word2vec`

`$ pip install -r requirements.txt`







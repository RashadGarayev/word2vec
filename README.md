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

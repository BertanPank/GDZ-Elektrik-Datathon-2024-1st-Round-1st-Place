Competition Name: Gdz Elektrik Datathon 2024

Competition Link: https://www.kaggle.com/competitions/gdz-elektrik-datathon/leaderboard

Result: 1st/192 (Round Canceled)

---------------------------------------------------------------------------------------------

!!!

[TR]

İlk roundun kodlarını kayıtlı tutmadığım için final aşaması bittikten sonra hatırladığım kadarıyla ilk round çalışmamızı üretmeye çalıştım.
Hemen hemen aynı notebooku oluşturabildiğimi düşünüyorum ama final roundunun datasını kullanarak yaptığım için bazı minör sütun ismi ve tarih değer farkları var.

[EN]

Since I didn't save the code from the first round, I tried to reproduce our first round work from memory after the final phase ended. I believe I managed to create almost the same notebook, but there are some minor differences in column names and date values because I used the data of the final round.

!!!

--------------------------------------------------------------------------------------------

[TR]

Problem: İzmir ve Manisa ilçelerindeki toplam 47 ilçenin gelecek bir aydaki günlük trafo kesinti miktarının tahminlenmesi.

Yaklaşımımız:

Özellik çıkarımları:

-Fourier Döngüleri

-Günlük hava durumu tahminlerinden istatistiksel (min, max, mean, median, std) özellik çıkarımı

-Rüzgar yönü ve şiddetini birleştiren featurelar oluşturulması

-İlçelerin günlük hava durumu tahminlerinden istatistiksel (min, max, mean, median, std) özellik çıkarımı

-Bayram özelliği

Modelleme:

-Oldukça fazla model denedik. Hızlıca hangi modellerin iyi performans gösterdiğini görmek için Autogluon.tabular, Autogluon.timeseries ve Pycaret AutoML kütüphhanelerini kullandık.

-Sonuç olarak ağaç modellerinin çok daha iyi pperformansa sahip olduğunu gördük ve Autogluon.tabular kullanmaya devam ettik.

-Eğer etap devam etseydi muhtemelen daha kompleks modellere yönelirdik.

---------------------------------------------------------------------------------------------------------------------------

[EN]

Problem: Forecasting the daily transformer outage amount for the next month in a total of 47 districts in İzmir and Manisa.

Our Approach:

Feature Engineering:

-Fourier Cycles

-Statistical feature extraction (min, max, mean, median, std) from daily weather forecasts

-Statistical feature extraction (min, max, mean, median, std) from daily weather forecasts for districts

-Creating features that combine wind direction and intensity

-Holiday feature

Modeling:

-We tested a lot of models. To quickly see which models performed well, we used the AutoML libraries Autogluon.tabular, Autogluon.timeseries, and Pycaret.

-As a result, we found that tree models had much better performance, so we continued to use Autogluon.tabular.

-If the stage had continued, we would likely have turned to more complex models.

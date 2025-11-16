🇺🇸 README – English (🇹🇷Türkçe Aşşağıda)
Bitcoin Price Direction Prediction – Machine Learning Project

This project focuses on predicting the next 1-hour price movement of Bitcoin (up or down).
Since cryptocurrency markets are highly volatile, short-term prediction is both difficult and interesting. My goal was to explore how traditional ML models and deep learning models perform on real market data.

🎯 Purpose of the Project

The main objectives were:

Predict the next hourly price direction of Bitcoin,

Compare multiple ML and DL models,

Apply preprocessing, feature selection, and model evaluation steps,

Build a complete end-to-end machine learning pipeline.

📂 Dataset

I used the Bitcoin Pulse Market Trends Dataset from Kaggle.
It contains hourly:

open/high/low/close prices,

trading volumes,

several financial index values
for BTC, ETH, BNB, DOGE, and other assets.

Total size: 17,515 rows – 131 features
There were no missing values in the dataset.

🔧 Data Preparation

The Datetime column was split into:
year, month, hour, day_of_week.

These were converted with Label Encoding and One-Hot Encoding.
All other features were already numerical.

🔍 Feature Selection

A total of 10 feature selection methods were applied.
These included SelectKBest, Mutual Information, RandomForest Importance, L1 Logistic Regression, RFE, XGBoost, and LightGBM.

Most methods highlighted volume-related features and open/close prices as the most influential variables.

📊 Correlation Analysis

A correlation heatmap was generated to explore relationships between assets.
Crypto-to-crypto correlations were naturally high, while financial indices showed weaker connections.

🤖 Models Used

Eight models were trained and compared:

Machine Learning:

Decision Tree

Random Forest

KNN

SVM

Logistic Regression

Deep Learning:

DNN

CNN

LSTM

Performance metrics such as accuracy, precision, recall, f1-score, training time, and inference time were recorded.

📝 Results

Overall accuracy values were not high. This is expected because short-term Bitcoin movement is difficult to predict using only price and volume data.

CNN achieved the highest accuracy (51.56%) but predicted almost all samples as the same class.

Random Forest performed more balanced, but its accuracy remained close to random chance (~50%).

General Conclusion:
The dataset lacks strong predictive signals for directional Bitcoin forecasting. Incorporating additional data sources (sentiment, on-chain metrics, macro signals, etc.) would likely improve the model significantly.

📚 References

Kaggle Dataset

Scikit-learn

TensorFlow

XGBoost

LightGBM
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
🇹🇷 README – Türkçe
Bitcoin Fiyat Tahmini – Makine Öğrenmesi Projesi

Bu proje, Bitcoin’in bir sonraki saatlik fiyat hareketinin (yükseliş veya düşüş) tahmin edilmesi üzerine kuruludur. Kripto paraların oldukça oynak bir yapısı olduğu için kısa vadeli tahmin yapmak hem zor hem de ilgi çekici bir problem. Ben de bu projede gerçek piyasa verilerini kullanarak farklı makine öğrenmesi ve derin öğrenme modellerinin bu konuda ne kadar başarılı olabileceğini test etmek istedim.

🎯 Projenin Amacı

Bu çalışmada temel hedefim:

Bitcoin’in bir saat sonraki fiyat yönünü tahmin etmek,

Çeşitli ML ve DL modellerini karşılaştırmak,

Veri ön işleme, özellik seçimi ve model değerlendirme adımlarını uçtan uca uygulamak,

Gerçek bir veri bilimi sürecinin nasıl işlediğini göstermekti.

📂 Kullanılan Veri Seti

Projede Bitcoin Pulse Market Trends Dataset (Kaggle) kullanıldı.
Bu veri seti; Bitcoin, Ethereum, BNB, Dogecoin gibi birçok kripto paranın:

saatlik fiyatları (open/high/low/close),

hacimleri,

bazı finansal endeks değerlerini
içeriyor.

Toplam: 17515 satır - 131 özellik
Eksik veri bulunmadığı için ek bir doldurma işlemi yapılmadı.

🔧 Veri Hazırlama Süreci

Projeyi yaparken ilk iş olarak Datetime sütununu year, month, hour, day_of_week olarak ayırdım.
Böylece zaman bileşenlerinin model üzerindeki etkilerini ayrı ayrı görebildim.

Kategorik olan zaman değişkenleri:

Label Encoding

One-Hot Encoding

yöntemleriyle dönüştürüldü.

Ardından karakter sütunu hariç tüm veriler sayısal halde modele hazır hale getirildi.

🔍 Özellik Seçimi

Bu projede özellikle vurgulamak istediğim nokta, 10 farklı özellik seçimi tekniği kullanmış olmam.
Bunların arasında SelectKBest, Mutual Information, RandomForest Feature Importance, L1 Logistic Regression, RFE, XGBoost, LightGBM gibi yöntemler var.

Bu yöntemlerin çoğu, özellikle hacim (volume) ve açılış-kapanış fiyatlarını en belirleyici özellikler olarak öne çıkardı.

📊 Korelasyon İncelemesi

Veri setindeki tüm sayısal değişkenler arasındaki ilişkileri incelemek için bir korelasyon matrisi oluşturdum.
Bazı kripto paraların fiyat ve hacimlerinin doğal olarak birbirleriyle yüksek korelasyona sahip olduğu görülürken, finansal endekslerle ilişkileri daha zayıf çıktı.

🤖 Kullanılan Modeller

Toplamda 8 model çalıştırıldı:

Makine Öğrenmesi:

Decision Tree

Random Forest

KNN

SVM

Logistic Regression

Derin Öğrenme:

DNN

CNN

LSTM

Her model için accuracy, precision, recall, f1-score, eğitim süresi ve tahmin süresini kaydettim.

📝 Sonuçlar

Modeller genel olarak çok yüksek doğruluk vermedi. Bunun ana nedeni, Bitcoin gibi volatil bir varlığın sadece fiyat ve hacim bilgileriyle kısa vadeli tahmininin zor olması.

CNN, %51.56 accuracy ile en yüksek sonucu verdi.
Fakat sınıf dağılımına baktığımda model neredeyse tüm örnekleri aynı sınıfa tahmin etmiş.

Random Forest, daha dengeli tahmin yaptı ama doğruluk %50 civarında kaldı.

Genel İzlenim:
Veri setindeki özellikler Bitcoin'in bir saat sonraki fiyat yönünü güçlü şekilde temsil etmiyor. Ek veri kaynakları eklenerek model çok daha iyileştirilebilir.

📚 Kaynaklar

Kaggle – Bitcoin Pulse Market Trends Dataset

Scikit-learn

TensorFlow

XGBoost

LightGBM

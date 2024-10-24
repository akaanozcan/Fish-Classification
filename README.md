# Fish-Classification

9 farklı deniz ürünü türünün fotoğrafları içeren dataset üzerinde yapay sinir ağlarıyla sınıflandırma yaptım. İlk olarak yeni bir dataframe oluşturup içinde path ve label adlı iki sütun oluşturdum. Path sütunu fotoğrafların dosya yolunu, label ise deniz ürününün türünü gösteriyordu. Datasetin içinden onları gerekli sütunlara aktardım. 

Daha sonra dataset üzerinde çeşitli incelemeler yaptım. NULL değer kontrolü, her türden kaç tane veri olduğunu yazılı ve görsel olarak oluşturdum. Ayrıca her türden birer tane görüntü gösterdim. Bu fotoğraflar png uzantılı olduğundan onları numerik değere çevirdim. Keras özelliklerini kullanarak 128x128 görüntü oluşturdum, sayısal diziye çevirdim ve normalize ettim. 

Daha sonra verileri test, train ve validation olarak üçe ayırdım. One hot encoding işlemi uyguladım tüm verilere. Keras'tan Sequential ile model oluşturdu (2 gizli katmana sahip). Modeli derledim, early stopping uyguladım. Modeli fit edip result değişkeninde sakladım. 

Train ve validation setlerinin performansını karşılaştırdım. Bir loss grafiği, bir tane de accuracy grafiği oluşturdum. En sonda test seti ile tahmin yapıp loss ve accuracy değerlerini aldım.

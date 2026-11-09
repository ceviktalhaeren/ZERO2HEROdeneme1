# Rapor

**Ad Soyad:**TALHA EREN ÇEVİK
**Numara:**748

## 1. Problem Analizi
<!-- Problemi kendi cümlelerinizle yazın. -->
Kişiden doğru ve yanlış cevap sayısını alıp hata kontrolü yapar eğer hata çıkmıyor ise net ve boş sayısını hesaplar 
nete göre başarı durumunu yazdırır

## 2. Girdi - İşlem - Çıktı

**Girdiler:**
-doğru sayısı,yanlış sayısı

**İşlemler:**
-net sayısı,boş sayısı

**Çıktılar:**
-başarı durumu,net ve boş sayısı

## 3. Matematiksel Formüller
net = dsay -( ysay/4.0)
bos = 20-(dsay+ysay)

-

## 4. Sözde Kod (Pseudocode)

```
1.başla kullanıcıdan doğru sonra yanlış sayısını alır ardından hata kontrolü yapar eper doğru ve yanlış sayısı 20 den büyük veya doüru ve yanlış
sayısı 0 dan küçük ise hata yazdırılır
2.hata yok ise net ve boş sayısı hesaplanır ve yazdırlır

3.nete göre başarı durumu belirlenir 15 netten fazla ise çok iyi yazdırlır
15 ile 10 arasında ise iyi
5 ile 10 arasında ise ortalama
5 den düşük ise geliştirilmeli yazdırlıır
```

## 5. Akış Şeması


<img width="563" height="403" alt="image" src="https://github.com/user-attachments/assets/de54ec09-fd11-4a7c-9df0-4eb02947cd54" />

## 6. Başarı Durumu Koşulları
<!-- Koşulları hangi sırayla ve hangi operatörlerle yazdığınızı, nedenini açıklayın. -->
if net > 15 ise yani ilk olarak netin 15 den büyük olup olmadığına bakar
sonrasında if else 10 ile 15 arasında mı diye sorar çünkü 15 den fazla değil ise bu aralıkta olup olmadığını sorgular
sonrasında yine if else ile 5 ile 10 arasında olup olmadığına bakar
en son hiç biri değilse else kolundan ilerler


## 7. Test Sonuçları

| Doğru | Yanlış | Beklenen | Programın sonucu | Doğru mu? |
|---|---|---|---|---|
| 20 | 0 | Net 20, Çok iyi | Çok iyi  |evet |
| 15 | 4 | Net 14, İyi | İyi |evet |
| 10 | 8 | Net 8, Orta | Orta| evet|
| 5 | 0 | Net 5, Geliştirilmeli |Geliştirilmeli |evet |
| 0 | 20 | Net -5, Geliştirilmeli |Geliştirilmeli |evet |
| 10 | 10 | Net 7,5, Orta | Orta| evet|
| 15 | 10 | Geçersiz giriş |hata | evet|
| 12 | 9 | Geçersiz giriş |hata | evet|
| -1 | 5 | Geçersiz giriş |hata | evet|

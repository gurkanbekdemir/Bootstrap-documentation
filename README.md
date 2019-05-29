# Bootstrap'e giriş

Bugun Sizlerle Bootstrap adlı CSS(Cascade Style Sheet) Framework'unu Ögrenecegiz.

Öncelikle Kullanacağımız Dosyaları <a href="https://getbootstrap.com">Bootstrap Üzerinden indirelim.</a>
![image](https://user-images.githubusercontent.com/48087914/58375561-751d0400-7f5e-11e9-94f5-13b435e296dd.png)
Bootstrap'i 2 Şekilde kullanabiliriz. Bunlar CDN üzerinden dosyaları çekerek veya kaynak dosyalarını proje dosyamıza indirerek yapılabilir.

## CDN
```html
<!-- CSS ve JS -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>


<!-- JQuery ve PopperJs-->
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
```

## Kaynak Dosya İndirmek

![image](https://user-images.githubusercontent.com/48087914/58375654-8ebf4b00-7f60-11e9-96ca-7923aea9d352.png)


## Kurulum
Gerekli Klasörleri Proje dosyamıza atıyoruz.
![image](https://user-images.githubusercontent.com/48087914/58375761-43f30280-7f63-11e9-93c3-3ca3eb01b2fe.png)


## Başlangıç 

Klasik HTML Taglerimizi atıyoruz.
```html
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>
```
Bootstrap css ve js dosyasını içeri alıyoruz.
```html
<link rel="stylesheet" href="css/bootstrap.css">
<script src="js/bootstrap.min.js"></script>
```
### Responsive Nedir

   Telefon, Televizyon,Telefon,Tablet gibi ürünlerinizde sitenizin otomatik olarak boyutlandırılmasını sağlar.
## Containers 
Container'lar Responsive tasarım İçin gerekli Grid sistemini barındıran yapıdır.


2 Tip Kullanımı vardır 

Container ve Container Fluid

## Container 
Her zaman %100 Görünüm de gösterim sağlar.

## Container Fluid 
Tam Genişlikli bir container için kullanılır. sıvı gibi  tüm genişliği kaplar.


## Grid Sistemi

Tarayıcıda Görüntülenen ekran Bootstrap üzerinde 12 parçaya bölünmüştür. Row ve Col olarak adlandırılmıştır.

Grid sisteminde tüm taşınabilir cihazlar için ayrı terimler tanımlanmıştır.

Col tanımlar iken 2 şeye bakılır

1- Hangi Ekran Tipi

2- Sutun Genişligi

## Ekran Tipleri
1- Ekstra Küçük cihazlar  = xs

2- küçük ve orta cihazlar =sm

3- orta cihazlar için = md

4- büyük cihazlar için = lg

## Offset ve Push

CSS'deki Margin gibidir. Marginin işlevini CSS'de hatırlayacak olursak diger nesnelerden belirttigimiz px,pt vb değer kadar uzaklaştırmaya yarıyor du 

```html
<div class="col-md-10 col-md-offset-1">
```
Yazdığımızda 10 Sutun genişliginde bir sutun açıyoruz.
offset-1 kullandığımız için her iki yanına 1 sutunluk boşluk bıraktı ve 12 lik ızgara yapısını tamamlamış bulundu.

```html
<div class="col-md-9 col-md-push-3">
```
Yazdığımızda Sadece sol taraftan 3 Sutunluk ittirme yapabiliyoruz. 


# Başlık
Normal HTML etiketlerinde h1 den başlayarak h6 ya kadar giden başlık etiketleri bulunur. Kullanımı Aşağıdaki gibidir.
```html
<h1>Bootstrap</h1>
<h6>Bootstrap</h6>
```
Bootstrap ile bunu başlık etiketi almadan Class içinde  kullanabiliriz.
```html
<p class="h1">h1. Bootstrap Başlığı,d</p>
```
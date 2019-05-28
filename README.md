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
<p class="h1">h1. Bootstrap Başlığı</p>
```
veya Bootstrap'in kendi Responsive Başlıklarını kullanabiliriz.
```html
<h1 class="display-1">Başlık 1</h1>
<h1 class="display-2">Başlık 2</h1>
<h1 class="display-3">Başlık 3</h1>
<h1 class="display-4">Başlık 4</h1>
```
# Paragraf
Paragrafları Öne çıkarmak için lead Class'ını kullanalım.

```HTML
<p class="lead">
  Sonunda, ԁüşmanlarımızın sözlerini değil ԁostlarımızın sessizliğini hatırlayacağız. Martin Luther King
</p>
```

# Sıralı Yazı Elementleri

```html
<p>You can use the mark tag to <mark>highlight</mark> text.</p>
<p><del>This line of text is meant to be treated as deleted text.</del></p>
<p><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p><u>This line of text will render as underlined</u></p>
<p><small>This line of text is meant to be treated as fine print.</small></p>
<p><strong>This line rendered as bold text.</strong></p>
<p><em>This line rendered as italicized text.</em></p>
```
Sıra ile Ekranda göreceğiniz görüntü bu olacaktır.
![image](https://user-images.githubusercontent.com/48087914/58444469-1fcd2800-8101-11e9-8568-47edab5473ad.png)

# Kısaltmalar
Bootstrap Kısaltmalar için bize abbr etiketini ve initialism Class'ını tanımlamış
```html
<p><abbr title="attribute">attr</abbr></p>
<p><abbr title="HyperText Markup Language" class="initialism">HTML</abbr></p>
```
initialism sayesinde daha küçük bir font yazısı ile görüntüleme sağlıyoruz.

abbr etiketi ile üzerine geldigimizde soru işareti çıkararak Uzun Adını görmemizi sağlıyor.

# Alıntı Cümleleri
Bir alıntı yaptığımızda belirtmek için hazır bir etiket  olan Blockquote yardımımıza koşuyor.

```html
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
```
Ekranda göreceğiniz Görüntü ise şöyledir;
![image](https://user-images.githubusercontent.com/48087914/58444826-80a93000-8102-11e9-9873-bdf5ee480ab1.png)
Aynı şekilde yazı kısmını sağ sol ve orta olmak üzere yerlerini değiştirmek için blockquote text- yazıp yönünü belirtmeniz yeterli.

# Listeler
Biliyorsunuz ki Klasik HTML CSS üzerinde UL ve Li kullanarak listeler oluşturabiliyoruz, fakat bunun stilini değiştirmek istedigimizde CSS'den veya HTML etiketlerinden Liste tipini değiştirmeliyiz.

Bootstrap bunu bir class ile Çözümlüyor

```html
<ul class="list-unstyled">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
```
![image](https://user-images.githubusercontent.com/48087914/58444980-48562180-8103-11e9-92be-5ffe9413efec.png)

<h5>Gördügünüz gibi ilk kısımda list-unstyled Classını kullandığımız için Liste Etiketi gelmedi.</h5>

# Resimler
Resimleri Sayfaya doldurmak için img-fluid class'ı kullanılır
```html
<img src="..." class="img-fluid" alt="Responsive image">
```
veya Kapak Fotoğrafı için  img-thumbnail kullanabiliriz.
```html
<img src="..." alt="..." class="img-thumbnail">
```
# Tablolar
Tabloları günlük hayatta Listelemek için her zaman kullanırız. Bootstrap bize burda çok güzel özellikler sunuyor.Hadi inceleyelim.

Varsayılan Tablo tanımı

```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```
<h5>Tablo Görüntüsü böyle görünecektir.</h5>

![image](https://user-images.githubusercontent.com/48087914/58445543-b4d22000-8105-11e9-8832-559696102776.png)

Table Class'ı içerisine table-dark Yazarsanız Tablo Tamemen Siyah olur
<h5>Ve Tablo Böyle görünecektir.</h5>

![image](https://user-images.githubusercontent.com/48087914/58445618-fbc01580-8105-11e9-8182-cd2c56da1ad2.png)

<h5>Ve Tablo Başlıklarının rengini beyaz ve siyah yapabilirsiniz</h5>
Sadece thead Etiketinin class'ına thead-light veya thead-dark Yazmanız yeterli.
<h5>Ve Tablo Başlıkları Şöyle görünür.</h5>

![image](https://user-images.githubusercontent.com/48087914/58445901-36767d80-8107-11e9-97dd-ad28b3f8cc5c.png)

<h5> Zebra Cizgilerini de yapabiliriz.</h5>
<h5> bunun için table-striped class'ını eklememiz yeterlidir.</h5>

```html
<table class="table table-striped">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
```
<h5> Sonuna table-dark eklerseniz Siyah Gri bir tasarıma sahip olur </h5>

![image](https://user-images.githubusercontent.com/48087914/58446241-a9ccbf00-8108-11e9-8f3f-6a77267f8d13.png)

<h5> Tablonun Hücre çizgilerini kaldırmak isterseniz table-borderless eklemeniz yeterlidir. hücre çizgileri kaybolacaktır.

![image](https://user-images.githubusercontent.com/48087914/58446742-7ee36a80-810a-11e9-9e5d-500081a1a1c5.png)

<h5> Üzerine geldigimizde renk değişmek için ise table-hover Classını kullanmamız yeterli. <h5>

![image](https://user-images.githubusercontent.com/48087914/58446768-96225800-810a-11e9-8266-3bebdd3af2fd.png)

<h3> Küçük Tablolar </h3>

<h5>Küçük bir tablo yaratmak için table-sm kullanmamız yeterli oluyor.</h5>

![image](https://user-images.githubusercontent.com/48087914/58446821-e0a3d480-810a-11e9-9970-baaa4ad8a902.png)

 <h2> Renkler</h2>
<h5>Tablo içi renkledirmek için aşagıdaki renk class'larını deneyebiliriz</h5>

```html
!-- On rows -->
<tr class="table-active">...</tr>

<tr class="table-primary">...</tr>
<tr class="table-secondary">...</tr>
<tr class="table-success">...</tr>
<tr class="table-danger">...</tr>
<tr class="table-warning">...</tr>
<tr class="table-info">...</tr>
<tr class="table-light">...</tr>
<tr class="table-dark">...</tr>

<!-- On cells (`td` or `th`) -->
<tr>
  <td class="table-active">...</td>
  
  <td class="table-primary">...</td>
  <td class="table-secondary">...</td>
  <td class="table-success">...</td>
  <td class="table-danger">...</td>
  <td class="table-warning">...</td>
  <td class="table-info">...</td>
  <td class="table-light">...</td>
  <td class="table-dark">...</td>
</tr>
```
<h5>Sırasıyla Renklerimiz</h5>

![image](https://user-images.githubusercontent.com/48087914/58446914-43956b80-810b-11e9-99ef-e0042da1085c.png)

<h5>Karanlık Temadaki Renklerimiz </h5>

```html
<!-- On rows -->
<tr class="bg-primary">...</tr>
<tr class="bg-success">...</tr>
<tr class="bg-warning">...</tr>
<tr class="bg-danger">...</tr>
<tr class="bg-info">...</tr>

<!-- On cells (`td` or `th`) -->
<tr>
  <td class="bg-primary">...</td>
  <td class="bg-success">...</td>
  <td class="bg-warning">...</td>
  <td class="bg-danger">...</td>
  <td class="bg-info">...</td>
</tr>
```
<h5> Sırasıyla Renklerimiz böyle görünecektir.</h5>

![image](https://user-images.githubusercontent.com/48087914/58447043-c5859480-810b-11e9-8c6e-e5c76b4a1916.png)

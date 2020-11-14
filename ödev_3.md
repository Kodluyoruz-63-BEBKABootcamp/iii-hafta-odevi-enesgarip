#### .Net kodu nedir ve nasıl derlenir?

![](C:\Users\Garip\Desktop\Untitled.png)

.Net Framework farklı dillerin aynı çatı altında çalışmasını sağlar. .Net bunu CLR(Common Language Runtime) sayesinde yapar. Örneğin C# programı derleyicisi tarafından MSIL dosyasına dönüşür. Fakat bu dosyayı çalıştırmak için JIT'ye ihtiyaç vardır. JIT'den çıkan program artık makine dilindedir.

#### Roslyn compiler ne işe yarar?

Roslyn, .Net Compiler Platform'un takma adı olarak bilinen, açık kaynak compiler ve kod analiz API 'dır. C#, Visual Basic .Net dilleri içindir.Roslyn, kodun lexical analizi , semantic(anlamsal) analizi için modüller sunar.

#### Restful servisler nasıl çalışır? Alternatifleri nelerdir ve nasıl çalışırlar?

Rest, client-server arasındaki haberleşmeyi sağlayan HTTP protokolü üzerinde çalışan bir mimaridir. Rest, servis yönelimli yazılımlarda kullanılan bir transfer yöntemidir. Rest mimarisini kullanan servislere Restful servisler denir.

Bir API’nin RESTful API mi, yoksa REST API mi olduğu ayrımını yapmak adına bu listeye hakim olmanız tavsiye edilir:

- **İstemci ve sunucu:** İstemci front-end, sunucu ise back-end ile ilgilenir. Her ikisi birbirinden bağımsız olarak değiştirilebilir.
- **Durumsuzluk:** İstemcinin sorgu ve oturum durumuna dair depolama verileri hiçbir sunucu üzerinde barındırılmaz.
- **Önbellekleme:** İstemciler performansı arttırmak için yanıtı *(tıpkı bir internet sayfasının statik elementi gibi)* önbellekleyebilirler.
- **Tabaklı sistem:** İstemci sondaki sunucu veya aradaki süreç boyunca bir aracıya bağlı olup olmadığını söyleyemez.
- **Talep üzerine kod:** Sunucular, istemcinin fonksiyonelliğini geçici olarak icra ederek kod yollayabilir, genişletebilir ya da özelleştirebilir.

#### Extension method nedir? Nasıl yazılır?

Extension method mevcut class ve yapılar üzerinde değişiklik yapmadan genişletilmiş metod yazabilmemizi sağlar.Extension metodları kullanacağımız kaynak koda, using anahtar kelimesini kullanarak eklediğimizde bu metodları kullanabiliriz.Extension methodlar statik methodlardır.

#### MVC'nin alternatifleri nelerdir?

MVC'nin de bazı sorunları vardır. Bu sorunlar başlıca şunlardır.

* MVC için durum bilgisi önemlidir. View Model ile durumsal olarak bağlıdır bu sayede Model View'i değişiklikler sonucunda güncelleyebilir.
* MVC tek bir yoruma sahip değildir.

###### *Alternatifleri*

* HMVC ---> Hierarchical Model View Controller
* MVVM ---> Model View View Model
* MVP ---> Model View Presenter
* MVA ---> Model View Adapter
* PAC ---> Presentation Abstraction Control
* RMR ---> Resource Method Representation
* ADR ---> Action Domain Responder

#### Architectural pattern nedir? Neden ihtiyaç duyuyoruz?

Architectural pattern, yazılım mimarisinde sıklıkla karşılaşılan bir soruna tekrar tekrar kullanılabilir bir çözüm sunar. Design Pattern lardan farklı olarak yazılımın her yerine yayılmış olan problemleri çözmeyi hedeflemektedir.

#### ViewData, ViewBag, TempData farkları nelerdir? Çalıştığımız proje üzerinde başka bir branch açarak bunları deneyiniz?

ViewData ve ViewBag aynı amaç için kullanılırlar. Amaçları controller'dan view'e data transferi yapmaktır.

ViewData dictionary of objectdir. Elemanlarına key ile ulaşılabilir. ViewBag ise dinamiktir. 

TempData veriyi geçici olarak tutar. TempData bize veriyi controllerlar arasında veya actionlar arasında transfer etmede yardımcı olur. Fakat HTTP isteği süresi kadar veriyi tutarlar. Bu veriyi istek tamamlandıktan sonra ulaşabilmek için TempData.Keep() methodunu kullanmamız gereklidir. 

#### KAYNAKÇA

https://archive.codeplex.com/?p=roslyn

https://en.wikipedia.org/wiki/Roslyn_(compiler)

https://wmaraci.com/nedir/rest-api#:~:text=REST%20API%2C%20geli%C5%9Ftiricilerin%20HTTP%20protokol%C3%BCn%C3%BC,Aktar%C4%B1m%C4%B1%20olarak%20T%C3%BCrk%C3%A7ede%20de%20kullan%C4%B1l%C4%B1r.

https://medium.com/@serkan22789/c-extension-method-nedir-16dde50f9630

https://blog.ircmaxell.com/2014/11/alternatives-to-mvc.html

https://towardsdatascience.com/10-common-software-architectural-patterns-in-a-nutshell-a0b47a1e9013

https://medium.com/architectural-patterns/architectural-patterns-mimari-%C3%B6r%C3%BCnt%C3%BCler-2e945dc761b3

https://www.c-sharpcorner.com/blogs/viewdata-vs-viewbag-vs-tempdata-in-mvc1
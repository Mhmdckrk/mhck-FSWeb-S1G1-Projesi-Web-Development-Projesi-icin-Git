# Araştırma Soruları

Artık yeni iş yerindeki ilk görevini gerçekleştirmek için hazırsın! Kullandığımız araçları biraz daha iyi anlama zamanı. Yapman istenilen şey, bu dokümanı güncelleyerek, aşağıdaki soruları soruları cevaplaman. Böylece Git yapısına biraz daha aşina olmaya başlayacaksın.

Soruları cevaplarken takıldığın yerlerde [GitHub docs](https://docs.github.com/en)'u kullanabilirsin. Docs, (ingilizce documentation'ın kısaltılmış halidir) bir programı veya dilin nasıl kullanılacağını anlatan dokümandır. Yazılım dünyasında sıkça kullanılır. Bir yazılımcı olarak _zamanınızın büyük çoğunluğu da bu tarz dokümanları okumakla ve üzerinde çalışmakla geçecek_.

![READ THE DOCS](https://github.com/Workintech/FSWeb-S1G1-Projesi-Web-Development-Projesi-icin-Git/blob/main/read-the-docs-wit.gif?raw=true)

Eğer aradığın soruların cevapları GitHub docs'ta yoksa, Google'lama becerileriniz size yardımcı olacak. Google'ı iyi kullanabilmek de aslında büyük bir dikkat ve çalışma gerektiriyor. Zamanla bu konuda da daha iyileştiğini göreceksin :)

## Sorular

1. Git nedir?

Git bir projenin kaynak kod geçmişini takip etmeyi ve yönetmeyi sağlayan bir versiyon kontrol sistemidir. Git'i diğer versiyon kontrol sistemlerinden ayıran özelliklerinin başında brach yapısı gelmektedir. Brach yapısı ana koddan bağımsız olarak kodu çoğlatıp bu yeni branch üzerinde yeni fikirleri geliştirmeyi, geçmiş versiyonlar üzerinde çalışmayı branchleri birleştirmeyi sağlamaktadır.

2. Git ile GitHub arasında ne fark var?

Git bir versiyon kontrol sistemi olup lokalde bu kod verilerin(git repolarının) ve loglarının tutulmasını ve branchlar ile çoğalıtılarak üzerinde geliştirme yapılmasını sağlarken, Github işi biraz daha öteye taşıyarak bu Git repolarını internet ortamında public veya private olarak paylaşılması, değiştirilmesini ve birden fazla developerın bir projede herhangi bir karışıklığa meydan verden çalışabilmesini sağlamaktadır.

3. Neden bir branch oluşturuyoruz?

Bir projeye ait kodun ana yapısını bozmadan o kodu kopyalarak üzerinde değişiklikler ve geliştirmeler yapılmasını sağlamaktadır. Böylelikle bir proje için A-B testleri geliştirilebilmekte, yeni özellikler kolaylıkla eklenebilmekte ve kodun bakımı birden fazla developer tarafından rahatça yapılıp ardından bu güncellemeler ana branche eklenebilmektedir. 

4. Pull Request'in amacı nedir?

Github'ta başkasına ait bir projeyi kendimize aldığımızda -yani Fork ettiğimizde- ve bu kod üzerinde değişiklik yaptıktan sonra proje sahibinin bu kodu projesine çekip merge etmesi için çekme talebinde bulunmamıza "Pull request" diyoruz. Proje sahibi yaptığımız değişikliği inceleyip uygun görürse bu talebi kabul edip projesiyle bizim kodumuzu birleştirebilmektedir. 

5. Bir Branchten diğerine geçmek için kullandığın KOMUT nedir? Mesela `isim-soyisim` branch'inde çalıştığını hayal et ve main branch'ine geçmek istiyorsun, ne yaparsın?

Main branch'e geçmek için "git checkout master" komutunu kullanırım.

6. `git fetch`, `git merge` ve `git pull` arasındaki farklılıkları açıklayınız. Bu komutlar ne yapar açıklayınız.

git fetch, githubtan lokale çekmek istenilen verinin meta verisini - yani veri hakkındaki log benzeri bilgileri - almaya yarar. böylelikle kodları merge yapmadan önce değişiklerin görülmesini ve tutulmasını sağlamaktadır. Ardıdan git merge ile bunlar birleştirilir. "Git pull" ise "git fetch" ve "git merge" işlemleri tek seferde yapılmış olur. Ancak proje üzerinde birden fazla kişi çalışıyorsa "merge conflict" denilen çakışma hatasına sebep olabilmektedir. Bu yüzden bireysel projelerde "git pull" kullanmak daha hızlı ve kolay bir seçenektir. Birden fazla kullanıcı varsa git fetch ve merge kullanılması gerekmektedir.

7. Merge conflict nedir?

Aynı dosyadaki aynı kod parçasını iki farklı brachte değiştirilmesinin ardından merge yapılırsa merge conflict yani çakışma hatası verecektir ve merge işlemini yapmayacaktır.

8. Merge conflict'i nasıl çözeriz?

Burada git'in conflict olan yerleri manuel olarak incelenip ya ikisinden biri seçilmeli ya da birleştirmek istediğimiz gibi düzenlenmeli veyahut o kısım silinmelidir. Ardından commit yapılarak merge işlemi yapılmalıdır.


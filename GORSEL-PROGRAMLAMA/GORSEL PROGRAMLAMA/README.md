# 🎉 Public Holiday Tracker – Türkiye Resmi Tatil Sorgulayıcı



**C# Konsol uygulaması** ile 2023, 2024 ve 2025 yıllarına ait Türkiye’nin resmi tatillerini anlık olarak API üzerinden çekip kullanıcıya sunan bir projedir.



Bu proje; menü tabanlı bir yapı, kullanıcıdan dinamik input alma ve JSON verisini sınıflara dönüştürme mantığını öğretmeyi hedefler.



---



# 🧾 Özellikler



- [x] API’dan resmi tatil listesini çekme

- [x] JSON verisini `Holiday` sınıfına dönüştürme

- [x] Kullanıcının menü üzerinden seçim yapabilmesi

- [x] Yıla göre tatil listeleme

- [x] Tarihe göre tatil arama (gg-aa formatı)

- [x] İsme göre tatil bulma

- [x] Tüm yılların tatillerini tek listede gösterme

- [x] Dinamik kullanıcı input desteği



---



# 🚀 Çalıştırma



1. Projeyi bilgisayarınıza indirin (Clone/Download).

2. **Visual Studio** ile çözümü (`.sln`) açın.

3. `Program.cs` dosyasını çalıştırın (F5 veya Start).

4. Menü üzerinden istediğiniz sorgulamayı yapın.



---



# 📌 Kullanılan API



Uygulama, **Nager.Date API** uç noktalarından veri çeker:



* `https://date.nager.at/api/v3/PublicHolidays/2023/TR`

* `https://date.nager.at/api/v3/PublicHolidays/2024/TR`

* `https://date.nager.at/api/v3/PublicHolidays/2025/TR`



---



# 🧱 Holiday Sınıfı Yapısı



Gelen JSON verisi aşağıdaki C# sınıfına map edilir:



```csharp

class Holiday

{

    public string date { get; set; }

    public string localName { get; set; }

    public string name { get; set; }

    public string countryCode { get; set; }

    public bool fixed { get; set; }

    public bool global { get; set; }

}

```

# 🖥️ Uygulama Görünümü



Program çalıştırıldığında kullanıcıyı aşağıdaki menü karşılar:



```text

===== PublicHolidayTracker =====

1. Tatil listesini göster (yıl seçmeli)

2. Tarihe göre tatil ara (gg-aa formatı)

3. İsme göre tatil ara

4. Tüm tatilleri 3 yıl boyunca göster (2023–2025)

5. Çıkış



Seçiminiz: _

```





> **Not:** Her seçenekte kullanıcıdan gerekli bilgiler alınır ve sonuçlar konsol ekranında listelenir.



-----



# 📂 Proje Amacı



Bu proje aşağıdaki konuları pratik etmek amacıyla geliştirilmiştir:



  * 🌐 **API Tüketimi** (HttpClient)

  * 🔄 **JSON → C\# Model Dönüştürme** (Deserialization)

  * ⌨️ **Konsol Etkileşimi** (Kullanıcı Inputları)

  * 📋 **Algoritma Mantığı** (Menü Yapısı)



-----



# 📌 Geliştirici



| İsim | GitHub |

|---|---|

| **Yasin Balkan** | [TimaYT GitHub Profili](https://github.com/TimaYT) |



```

```


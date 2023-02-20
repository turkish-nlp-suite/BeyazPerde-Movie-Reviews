# BeyazPerde-Movie-Reviews

Beyazperde Movie Reviews offers Turkish sentiment analysis datasets that is scraped from popular movie reviews website Beyazprede.com. Currently there are 2 datasets, Top 300 Movies Dataset and All Movies Dataset. 

## Top 300 Movies

Top 300 Movies include reviews about best 300 movies of all the time. Here's the star rating distribution:

| star rating | count |
|---|---|
| 0.5  | 1.657 |
| 1.0  | 535 |
| 1.5  | 273 |
| 2.0  | 608 |
| 2.5  | 2.439 |
| 3.0  |2.277 |
| 3.5  | 5.550 |
| 4.0  | 13.248 |
| 4.5  | 10.077 |
| 5.0  | 17.351 |
| total | 54.015 |

As one sees, this dataset is highly unbalanced, number of 4 and 5 star ratings are much higher than 0, 1, 2 and 3 star reviews. This dataset offers the challenge of understanding the sentiment in a refined way, dissecting the positive sentiment into "very positive" or "okayish positive".

## All Movies Dataset

This dataset contains reviews about 4500 popular movies of all times. Here's the star rating distribution for this dataset:

 
| star rating | count |
|---|---|
| 0.5  | 3.635 |
| 1.0  | 2.325 |
| 1.5  | 1.077 |
| 2.0  | 1.902 |
| 2.5  | 4.767 |
| 3.0  |4.347 |
| 3.5  | 6.495 |
| 4.0  |9.486 |
| 4.5  | 3.652 |
| 5.0  | 7.594 |
| total | 45280 |

--------------------------------------

Each instance of the dataset is a JSON consisting of 

- movie URL
- movie name
- genre info
- description
- director info
- actors
- creators/producers
- music creators
- rating info
- a list of reviews, each element of the list is a review and a rating value in 0-5 scala.

Here's an example JSOn for you:

```
  {
    "url": "https://www.beyazperde.com/filmler/film-178014",
    "name": "Avatar: Suyun Yolu",
    "genre": [
      "Bilimkurgu",
      "Macera",
      "Fantastik",
      "Aksiyon"
    ],
    "desc": "Avatar serisinin 2009 yılında küresel bir fenomen haline gelen devam halkası; bu defa James Cameron'un yaratmış olduğu öykü evreninin hem kökenlerine iniyor hem de sınırlarını genişletmeyi hedefliyor. Avatar'da yaşanan olaylardan birkaç yıl sonra Jake ve Neytiri Pandora'da kendi ailelerini kurmuştur. Ancak onlar evlerini terk etmek zorunda kalır. Bu yüzden Jake ve Neytiri, suyun yüzeri ve altı dahil olmak üzere Pandora'nın dışındaki yerleri keşfetmeye başlar.",
    "directors": "James Cameron",
    "actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
    "creators": "James Cameron, Rick Jaffa, Amanda Silver, Amanda Silver, James Cameron, Rick Jaffa, Josh Friedman, Shane Salerno",
    "musicBy": "Simon Franglen, The Weeknd",
    "rating": {
      "totalRating": "4,3",
      "ratingCount": "187",
      "reviewCount": "45",
      "bestRating": "5",
      "worstRating": "0,5"
    },
    "reviews": [
      {
        "rating": "4,0",
        "review": "Filmi bugün Nişanlımla birlikte izleme şansım oldu. Avatarı ilk izlediğimde nedense çokta etkisinde kalmamıştım. bu filme de gittiğimde ilk filmi unutmuştum bile. Avatar 2 yi izleyince Avatar evreni ilgimi çekmeyi başardı. üçüncü filmi beklemiyorum desem yalan olur. Üçüncü Filmde fantastik ögelerden çok bilim kurgu yönünün ağır basması filmi daha anlamlı kılacağını düşünüyorum. Umarım üçüncü filmde yönetmen bu konuya önem verir. Onun dışında Film son zamanlarda izlediğim en naif en ahlaklı yapım diyebilirim. Ailecek gönül rahatlığıyla gidip izleyebilirsiniz. Günümüz yapımları gibi saçma sapan cinsel içerikli konuşmalardan, hareketlerden ibaret değildi. Filmde iki önemli mesaj vardı bunlardan biri aile diğeri küresel iklim değişikliği yani Doğa. Hep doğaya hemde aile yaşantısına karşı çokça mesaj çokça replik barındıran anlamlı bir filmdi. (Aile olmak hem en büyük zaafımız hemde en büyük gücümüz.) Üç saat olmasına rağmen hiçbir sıkılmadım. Aksiyon ve Trajediyi harmanlayıp izleyiciye çok iyi aktarıldığını düşünüyorum. Görsel efekt çekim teknikleri karakterler ve mekanlar harikulade diyebilirim. Tek kusur gördüğüm şey keşke iyi ve kötünün savaşını sadece bir aile sorununa indirgemeyip bu sorunu gezegenin tüm sorunu olarak göstermesi daha ihtişamlı olabilirdi. Sonuçta düşmanlar gezegene sadece Jake için gelmiyordu gezegeni tümüyle işgal edip, sömürmek için geliyordu. Ayrıca çocuk karakterler filmin yarısından sonra biraz fazla filme dahil olmaya başladı, bu bazı seyircileri sıkmış olabilir. Neyse sonuçta James Cameron müthiş bir evren oluşturmuş, izlemeye değer."
      },
      {
      ....
      }
    ]
  }
```



This work is supported by Google Developer Experts Program. Part of Duygu 2023 Fall-Winter collection, "Turkish NLP with Duygu"/ "Duygu'yla Türkçe NLP". All rights reserved.

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

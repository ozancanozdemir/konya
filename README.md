# konya


<img src="https://github.com/ozancanozdemir/konya/assets/33122288/3a0fc3a9-8411-4e6a-9bbb-6cc729a980cb" width="200">

This package is developed to access the datasets in [Konya Open Data Portal](https://acikveri.konya.bel.tr/)

## Installation

You can install the package from [CRAN.](https://cran.r-project.org/web/packages/konya/index.html)

```
install.packages("konya")
```

You can also install the package from GitHub.

```
remotes::install_github("ozancanozdemir/konya")
```

## Usage and Examples

```
> library(konya)
Welcome to konya package!
This is an unofficial R package for Konya Municipality Open Data Portal.
For more information, you can visit https://acikveri.konya.bel.tr/
```

The package has three main functions. You can list the all datasets by using ```list_data_names()``` 


```
list_data_names()
 [1] ""                                                                    
  [2] "bisiklet-tamir-ve-bakim-istasyonlari"                                
  [3] "paylasimli-kiralik-bisiklet-istasyonlari-konumlari"                  
  [4] "bisiklet-park-alanlari-ve-istasyonlarinin-konumlari"                 
  [5] "belediyetesisleri"                                                   
  [6] "kirsal-ve-kirsal-olmayan-tum-mahalleler"                             
  [7] "kati-atik-depolama-sahasi-ve-enerji-uretim-miktari"                  
  [8] "camiler"                                                             
  [9] "elkart-ile-saatlik-binis-sayilari"                                   
 [10] "elkart-toplam-yukleme-sayilari"                                      
 [11] "e-dolum-bakiye-yukleme-sayilari"                                     
 [12] "mezarliklar"                                                         
 [13] "saglik-tesisleri"                                                    
 [14] "okullar"                                                             
 [15] "geo-view-deneme"                                                     
 [16] "toplu-tasima-gtfs-verileri"                                          
 [17] "konyakartturlerinegorekullanimsayilari"                              
 [18] "hava-durumu-olcum-degerleri"                                         
 [19] "ucretsiz-wi-fi-kullanim-sayilari"                                    
 [20] "ilcelerden-toplanan-kati-atik-miktari"                               
 [21] "yillara-gore-konya-su-abone-sayilari"                                
 [22] ""                                                                    
 [23] "meyve-sebze-hal-fiyatlari"                                           
 [24] "aykome-fiyat-tarifesi"                                               
 [25] "konya-ilceleri"                                                      
 [26] "itfaiyenoktalari"                                                    
 [27] "konya-mahalleler"                                                    
 [28] "toplanma-alanlari"                                                   
 [29] "e-numarataj-ilce-bazli-yeni-bina-basvurusu"                          
 [30] "karatay2-istasyonu-hava-kalitesi-olcum-degerleri"                    
 [31] "karatay1-istasyonu-hava-kalitesi-olcum-degerleri"                    
 [32] "yillara-gore-ilcelerde-egitim-verilen-ciftci-sayilari"               
 [33] "erenkoy-istasyonu-hava-kalitesi-olcum-degerleri"                     
 [34] "eregli-istasyonu-hava-kalitesi-olcum-degerleri"                      
 [35] "bosna-istasyonu-hava-kalitesi-olcum-degerleri"                       
 [36] "karkent-istasyonu-hava-kalitesi-olcum-degerleri"                     
 [37] "laboratuvar-istasyonu-hava-kalitesi-olcum-degerleri"                 
 [38] "meram-istasyonu-hava-kalitesi-olcum-degerleri"                       
 [39] "merkez-trafik-istasyonu-hava-kalitesi-olcum-degerleri"               
 [40] "sarayonu-istasyonu-hava-kalitesi-olcum-degerleri"                    
 [41] "selcuklu-istasyonu-hava-kalitesi-olcum-degerleri"                    
 [42] "ilce-mahalle-bazli-meshur-urunler"                                   
 [43] ""                                                                    
 [44] "ilce-mahalle-bazli-sulak-alan-miktari"                               
 [45] "bina-tipine-gore-cikan-yangin-sayisi-istatistikleri"                 
 [46] "sehirde-gerceklesen-yangin-sayilari-ve-sebepleri"                    
 [47] "gerceklesen-itfai-olaylar"                                           
 [48] "konya-sehir-tiyatrosu-verileri"                                      
 [49] "kiralik-bisiklet-kullanim-verileri"                                  
 [50] "ilce-mahalle-bazli-kooperatif-mevcudiyeti"                           
 [51] "ilce-mahalle-bazli-dogrudan-satin-alinabilecek-urunler"              
 [52] "ilce-mahalle-bazli-en-cok-yetistirilen-urunler"                      
 [53] "ilce-mahalle-bazli-traktor-sayisi"                                   
 [54] "otobus-durak-varis-sureleri"                                         
 [55] "ilce-mahalle-bazli-bireysel-arazi-ortalamasi"                        
 [56] "ilce-mahalle-bazli-alternatif-yeni-urun-cesitleri-uretimi"           
 [57] "ilce-mahalle-bazli-devlet-destegi-faydalanma-cesitleri"              
 [58] "ilce-mahalle-bazli-endemik-bitkiler"                                 
 [59] "ilce-mahalle-bazli-talep-edilen-tarimsal-egitimler"                  
 [60] "ilce-mahalle-bazli-tibbi-ve-aromatik-bitki-yetistiriciligi"          
 [61] "ilce-mahalle-bazli-arkeolojik-alan"                                  
 [62] "ilce-mahalle-bazli-aricilik-durum-bilgisi"                           
 [63] "ilce-mahalle-bazli-beslenen-hayvan-turleri"                          
 [64] ""                                                                    
 [65] "ilce-mahalle-bazli-sulama-suyu-kaynagi-yonetimi"                     
 [66] "ilce-mahalle-bazli-hayvan-beslemede-kullanilan-urunler"              
 [67] "ilce-mahalle-bazli-sulanabilir-alanda-yetistirilen-urunler"          
 [68] "ilce-mahalle-bazli-sulama-suyu-kaynagi"                              
 [69] "ilce-mahalle-bazli-iyi-tarim-uygulamalari"                           
 [70] "ilce-mahalle-bazli-tarimsal-sulama-suyu-durum-bilgisi"               
 [71] "kobim-konya-bel-tr-gunluk-ziyaretci-sayisi"                          
 [72] "konya-mobil-uygulamasi-gunluk-ziyaretci-sayilari"                    
 [73] "komek-org-tr-gunluk-ziyaretci-sayisi"                                
 [74] "konyabuyuksehir-tv-gunluk-ziyaretci-sayisi"                          
 [75] "konyasehirtiyatrosu-com-gunluk-ziyaretci-sayisi"                     
 [76] "e-numarataj-ilce-bazli-adres-tespit-basvurusu"                       
 [77] "e-numarataj-yeni-bina-basvuru-sayisi"                                
 [78] "e-numarataj-adres-degisiklik-basvuru-sayisi"                         
 [79] "mezarliklar-defin-sayilari"                                          
 [80] "e-dolum-abonman-yukleme-sayilari"                                    
 [81] "otobus-hat-bilgisi"                                                  
 [82] "e-numarataj-bahce-suyu-basvuru-sayisi"                               
 [83] "e-numarataj-adres-tespiti-basvuru-sayisi"                            
 [84] "otopark-bilgileri"                                                   
 [85] ""                                                                    
 [86] "yillara-gore-tuketilen-su-miktari"                                   
 [87] "emekli-lokalleri"                                                    
 [88] "ilce-mahalle-bazli-gunes-enerji-santralleri-ve-kurulu-guc-miktarlari"
 [89] "e-numarataj-toplam-basvuru-sayilari-2021"                            
 [90] "e-hemsehrim-platformu-uye-istatistik"                                
 [91] "komek-merkez-konum"                                                  
 [92] "ilce-mahalle-bazli-konaklama-yeri-mevcudiyeti"                       
 [93] "ilce-bilgi-sistemi-talep-sayilari"                                   
 [94] "bilgehane-kayit-sayilari"                                            
 [95] "ucretsiz-wi-fi-hizmeti-erisim-noktalari"                             
 [96] "banka-karti-ile-binis-sayilari"                                      
 [97] "abonman-yukleme-sayilari"                                            
 [98] "mubis-konya-bel-tr-gunluk-ziyaretci-sayisi"                          
 [99] "bilgehane-merkez-konum-bilgileri"                                    
[100] "trafik-isiklari-konum-bilgisi"                                       
[101] "elektronik-yonlendirme-ekranlari-konum-bilgileri"                    
[102] "trafik-yogunluk-sensorleri-konum-bilgileri"                          
[103] "kobim-proje-bilgileri"                                               
[104] "komek-kayit-sayilari"                                                
[105] "atus-web-sayfasi-gunluk-ziyaretci-sayilari"                          
[106] ""                                                                    
[107] "kent-bilgi-sistemi-kbs-konya-bel-tr-gunluk-ziyaretci-sayilari"       
[108] "konya-com-tr-gunluk-ziyaretci-sayilari"                              
[109] "konya-bel-tr-gunluk-ziyaretci-sayilari"                              
[110] "atus-gunluk-sms-kullanim-sayilari"                                   
[111] "otobus-tarifeleri"                                                   
[112] "hava-kalitesi-istasyonlari-konum-bilgileri"                          
[113] "gurultu-olcum-istasyonlari-konum-bilgileri"                          
[114] "otobus-hat-durak-bilgisi"                                            
[115] "otobus-guzergah-bilgileri"                                           
[116] "konya-ilce-mahalle-bazli-yapi-sayisi"                                
[117] "aykome-verilen-kazi-ruhsati-sayisi"                                  
[118] "muhtarlik-bilgi-sistemi-ilce-bazli-talep-sayilari"                   
[119] "bilimmerkezi-ziyaretci-sayilari"                                     
[120] "e-dolum-toplam-sayilari"                                             
[121] "bakiye-yukleme-sayilari"                                             
[122] "akilli-durak-ekranlari-bilgileri"                                    
[123] "atik-su-aritma-tesisinde-uretilen-elektrik-enerjisi-miktari"     
```

You can get the data that you would like to have using ```get_data_from_konya(data_name)``` 

```
>get_data_from_konya("akilli-durak-ekranlari-bilgileri")
# A tibble: 184 × 3
   durak_no ekran_tipi enerji_tipi     
   <chr>    <chr>      <chr>           
 1 1003D    D          Güneş Enerjisi  
 2 1203A    D          Güneş Enerjisi  
 3 1409D    D          Güneş Enerjisi  
 4 17A      C          Güneş Enerjisi  
 5 2411D    C          Güneş Enerjisi  
 6 3D       A          Şebeke Elektriği
 7 3A       A          Şebeke Elektriği
 8 5D       A          Şebeke Elektriği
 9 6D       A          Şebeke Elektriği
10 7A       B          Şebeke Elektriği
# ℹ 174 more rows
# ℹ Use `print(n = ...)` to see more rows
``` 
You can search the data by using ```search_data_by_keyword(key_word).```

```
> search_data_by_keyword("bisiklet")
[1] "bisiklet-tamir-ve-bakim-istasyonlari"               
[2] "paylasimli-kiralik-bisiklet-istasyonlari-konumlari" 
[3] "bisiklet-park-alanlari-ve-istasyonlarinin-konumlari"
[4] "kiralik-bisiklet-kullanim-verileri"  
``` 

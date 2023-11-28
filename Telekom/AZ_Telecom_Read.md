## Telekom Müştəri Analizi
Mobil şəbəkəmizdə xidmət istifadəsini artırmağın necə planlaşdırılacağını öyrənmək üçün multisim istifadə tərəfindən təyin edilən abunələri müəyyənləşdirməyə çalımışıq.

Multisimmer, müştəri o deməkdir ki, eyni zamanda bir neçə operatorun xidmətlərindən istifadə edir.

Sizinlə multisimmer.parquet veri faylı təqdim edilib və bu fayl əsasında müştərilərin multisim istifadəsi tərəfindən ehtimal təxminləri təmin edən bir klasifikasiya növündə ML modeli qurmağınızı tələb edirik. Ehtimal eşik dərəcəsi __0.5__ olmalıdır.

Məxfilik məsələləri səbəbindən təmin edilmiş abunə kimlikləri və bəzi sütun adları maskalanmışdır.

Maskalanan sütun adları belə göstərilir: __var1, var2 ... .__

### Maskalanmayan sütunların təsviri

1) subscriber_id: hər bir abunəçinin unikal id nömrəsi 
2) trf: abunəçinin aktivləşdirilmiş tarifinin etiketlə kodlanmış adı
3) age: illərlə abunəçi yaşı
4) gndr: abunəçinin cinsi: M – kişi üçün, F – qadın üçün, U – naməlum üçün
5) tenure: günlərlə abunəçinin qalma müddəti
6) dev_man: abunəçinin cihazının istehsalçı adı
7) device_os_name: abunəçinin cihazının OS tipli istehsalı
8) is_dualsim:  1 - cihaz dulasim variantını dəstəkləyirsə, 0 - yoxsa
9) is_featurephone: 1 - cihaz funksiyalı telefon növüdürsə, 0 - deyilsə
10) is_smartphone: 1 - əgər cihaz smartfon növüdürsə, 0 - deyilsə
11) simcard_type: sim kartın texnologiya növü
11) region: abunəçi bölgəsinin etiket kodlu adı
12) target: 1 - abunəçi multisimmerdirsə, 0 - abunəçi yalnız bizim xidmətlərimizdən istifadə edirsə

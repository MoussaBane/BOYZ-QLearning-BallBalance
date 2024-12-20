# BOYZ-QLearning-BallBalance
Bilgisayar Oyunlarda Yapayzeka Dersinin Ödev 9

# Proje Kurulumu ve Başlangıç :
•	Unity Hub üzerinden yeni bir 3D proje oluşturun ve adını BallBalanceProject olarak belirleyin.

•	BallBalanceStarter projesini indirin ve projenize içe aktarın.

•	Scenes klasöründen "BallBalance" sahnesini açın.

# Ajanın (Platformun) Davranışı :
•	Gözlem: Ajan her iterasyonda topun mevcut durumunu (konum, hız, eğim) gözlemler.

•	Karar: Bu duruma göre, platformun sağa veya sola eğilmesi gibi bir aksiyon belirler.

•	Güncelleme: Eğer top düşerse, ajan bu hatasından öğrenir ve gelecekteki aksiyonlarını bu doğrultuda düzenler (Q-learning tablosu veya yapay sinir ağı ile).

# Oyun Mekanikleri :
Sahnedeki Elemanlar

•	Platform: Topun dengede kalacağı alan.

•	Border: Platformun sınırları (görünmez fakat çarpışma algılaması için etkin).

•	DroppedZone: Top düştüğünde tespitin yapıldığı alan.

Border ve DroppedZone Özellikleri

•	Mesh Renderer: Disabled (görünmez).

•	Tag: "drop" (düşme olaylarını algılamak için etiket).

Eğer top platform sınırlarını aşar ve "DroppedZone" bölgesine düşerse, bu bir başarısızlık olarak algılanır. Oyun yeniden başlar ve ajan, önceki denemelerdeki bilgileri kullanarak daha iyi aksiyonlar almaya çalışır.

# Oyunun Çalıştırılmış Hali:
![Ekran görüntüsü 2024-12-20 005716](https://github.com/user-attachments/assets/7103d632-7899-4619-b466-21c8aa71fd6a)

![Ekran görüntüsü 2024-12-20 021553](https://github.com/user-attachments/assets/2cc5707a-02e6-4d30-af39-b278f6144451)

![Ekran görüntüsü 2024-12-20 021710](https://github.com/user-attachments/assets/233b9f28-5d30-4991-84a2-21372e10cf03)

![Ekran görüntüsü 2024-12-20 021750](https://github.com/user-attachments/assets/06d8b409-eb2f-4efd-855e-b9c43d1707cb)

![Ekran görüntüsü 2024-12-20 021811](https://github.com/user-attachments/assets/e929b816-3720-438d-8660-9a5f0cdd5a07)


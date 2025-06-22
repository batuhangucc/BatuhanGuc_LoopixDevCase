LoopixDevCase, Unity 2022.3.53f1 ile geliştirilmiş, blok yerleştirme ve eşleştirme mantığına dayalı minimalist bir mobil bulmaca oyunudur.
Projede Background görsel ve ses efekt assetleri haricinde hiçbir hazır asset kullanılmamıştır.

⸻

Oynanış
	•	Oyuncu, “NOW” alanındaki bloğu sürükleyerek grid’e bırakır.
	•	Aynı türden 3 veya daha fazla blok yatay veya dikey olarak yan yana gelirse patlayarak yok olur.
	•	Her başarılı yerleştirmede skor artar, yeni bir blok “NEXT” alanında görünür.
	•	Grid tamamen dolduğunda Game Over ekranı görünür.

⸻

Kontroller
	•	Sürükle & Bırak: Bloklar grid’e sürüklenerek bırakılır.
	•	Restart: Oyunu sıfırlar ve baştan başlatır.
	•	Sound: Arka plan müziğini açıp kapatma seçeneği sunar.

⸻

Teknik Bilgiler
	•	Render Pipeline: Unity URP (Universal Render Pipeline) kullanıldı.
	•	Shader: Görsel efektler için Shader Graph ile özel materyaller ve shader’lar geliştirildi.
	•	Canvas: UI, 1080x1920 çözünürlük için “Scale With Screen Size” ayarıyla optimize edildi.
	•	Animasyon: Basit UI ve blok animasyonları Coroutine + Tween mantığıyla manuel olarak kontrol edildi.
	•	Ses: Patlama ve yerleştirme sesleri ile ambient bir arka plan müziği bulunur. Ses kontrolü kullanıcıya bırakılmıştır.
 	•	Android için build edilmiştir.
  •	Proje küçük ve sınırlı kapsamlı olduğu için tüm yapıyı event tabanlı kurmak yerine, doğrudan çağrılarla net ve sade bir iletişim tercih edilmiştir.
  •	Event sadece bazı özel durumlarda (örneğin draga and release) kullanılmıştır; ancak genel yapı event odaklı değildir.
  •	Kodlar mümkün olduğunca SOLID prensiplerine uygun ve sorumluluklar ayrılmış şekilde organize edilmiştir.
  

**Mikroservis Mimarisi ve Dağıtık Sistemler**

1. **Mikroservis Mimarisi Tasarımı**
   - **Mikroservislerin Temelleri:**
     - Mikroservis mimarisinin monolitik yapılara göre avantajları ve dezavantajları.
     - Bağımsız servislerin özellikleri: her servis kendi veri tabanı, iş mantığı ve API'leriyle ayrılmıştır.
   - **Modülerlik ve Sınırlar:**
     - Domain-Driven Design (DDD) ve Bounded Context kavramlarının mikroservis tasarımındaki önemi.
     - Sayaç verilerinin yönetimi için mikroservislerin domainlere göre bölümlendirilmesi.
     - Servisler arasında gevşek bağlılık ve yüksek iç tutarlılık sağlanması.
   - **Mikroservisler Arası İletişim:**
     - gRPC, HTTP/REST ve mesaj tabanlı iletişim yöntemlerinin karşılaştırması.
     - Servislerin senkron ve asenkron iletişim yöntemleriyle birbirleriyle haberleşmesi.
     - RabbitMQ ile mikroservisler arası mesajlaşma için en iyi uygulamalar.
   - **Veri Tutarlılığı ve Saga Pattern:**
     - Mikroservisler arasında dağıtık işlemler ve veri tutarlılığı sorunlarının çözümü.
     - Saga Pattern ile uzun süren işlemlerin yönetimi ve dağıtık sistemlerde eventual consistency.
     - Dağıtık transaction yönetimi ve rollback stratejileri.

2. **API Gateway ve Yük Dengeleme**
   - **API Gateway'in Rolü:**
     - Mikroservisler için merkezi bir erişim noktası olarak API Gateway’in önemi.
     - Kimlik doğrulama, rate limiting ve loglama gibi cross-cutting concern'lerin API Gateway'de yönetilmesi.
   - **API Gateway Tasarımı ve Uygulama:**
     - API Gateway’in seçimi (Kong, NGINX, Ocelot) ve deployment stratejileri.
     - API Gateway'de yönlendirme (routing) kurallarının ve load balancing’in yapılandırılması.
   - **Yük Dengeleme ve Trafik Yönetimi:**
     - Round-robin, weighted round-robin ve ip hash gibi yük dengeleme algoritmalarının uygulanması.
     - Dinamik yük dengeleme ve trafik yönlendirme stratejileri.
     - Trafiği analiz etmek ve yönlendirmek için API Gateway’in observability araçlarıyla entegrasyonu.
   - **Service Discovery ve API Gateway:**
     - Mikroservislerin API Gateway üzerinden otomatik olarak keşfedilmesi.
     - Consul, Eureka ve Kubernetes service discovery mekanizmaları ile API Gateway entegrasyonu.

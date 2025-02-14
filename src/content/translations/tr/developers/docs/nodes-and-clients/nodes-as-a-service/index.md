---
title: Hizmet olarak düğümler
description: Düğüm hizmetleri, bunların artıları ve eksileri ve popüler sağlayıcılara giriş düzeyinde bir genel bakış.
lang: tr
sidebar: true
sidebarDepth: 2
---

## Giriş {#Introduction}

Kendi [Ethereum düğümünüzü](/developers/docs/nodes-and-clients/#what-are-nodes-and-clients) çalıştırmak, özellikle başlarken veya hızlı ölçeklendirme yaparken zor olabilir. Sizin için optimize edilmiş düğüm altyapılarını çalıştıran [bir dizi hizmet](#popular-node-services) vardır, böylece bunun yerine uygulamanızı veya ürününüzü geliştirmeye odaklanabilirsiniz. Düğüm hizmetlerinin nasıl çalıştığını, bunları kullanmanın artılarını ve eksilerini açıklayacağız ve başlamakla ilgileniyorsanız sağlayıcıları listeleyeceğiz.

## Ön Koşullar {#prerequisites}

Düğümlerin ve istemcilerin ne olduğu konusunda henüz bir fikriniz yoksa, [Düğümler ve istemciler](/developers/docs/nodes-and-clients/)'e bakın.

## Düğüm hizmetleri nasıl çalışır? {#how-do-node-services-work}

Düğüm hizmeti sağlayıcıları, siz uğraşmayın diye sahne arkasında sizin için dağıtılmış düğüm istemcileri çalıştırır.

Bu hizmetler tipik olarak blok zincirine yazmak ve blok zincirinden okumak için kullanabileceğiniz bir API anahtarı sağlar. Bunlar genellikle Mainnet'e ek olarak [Ethereum test ağlarına](/developers/docs/networks/#ethereum-testnets) erişim içerir.

Bazı hizmetler, sizin için yönettikleri kendi özel düğümünüzü sunarken, diğerleri etkinliği düğümler arasında dağıtmak için yük dengeleyicileri kullanır.

Neredeyse tüm düğüm hizmetlerini entegre etmek aşırı derecede kolaydır: Kendi kendine barındırılan düğümünüzü değiştirmek veya hizmetler arasında geçiş yapmak için tek satırlık kod değişiklikleri yeterli olabilir.

Çoğu zaman düğüm hizmetleri çeşitli [düğüm istemcileri](/developers/docs/nodes-and-clients/#execution-clients) ve [düğüm türleri](/developers/docs/nodes-and-clients/#node-types) çalıştırarak tek bir API'de istemciye özel yöntemlere ek olarak tam düğümlere ve arşiv düğümlerine erişmenize olanak tanır.

Düğüm hizmetlerinin özel anahtarlarınızı veya bilgilerinizi saklamadığını ve saklamaması gerektiğini unutmamak önemlidir.

## Bir düğüm hizmeti kullanmanın faydaları nelerdir? {#benefits-of-using-a-node-service}

Bir düğüm hizmeti kullanmanın asıl faydası, düğümlere bakım yapmak ve yönetmek için uğraşmanız gerekmemesidir. Bu, altyapı bakımı konusunda endişelenmek yerine ürününüzü oluşturmaya odaklanmanıza olanak tanır.

Kendi düğümlerinizi çalıştırmak, depolamadan bant genişliğine ve mühendisliğe harcanan değerli zamana kadar çok pahalıya mal olabilir. Ölçeklendirirken daha fazla düğüm başlatmak, düğümleri en son sürümlere yükseltmek ve durum tutarlılığını sağlamak gibi şeyler, istediğiniz web3 ürününde kaynak oluşturma ve harcama konusundan sizi uzaklaştırabilir.

## Bir Düğüm Hizmeti kullanmanın eksileri nelerdir? {#cons-of-using-a-node-service}

Bir düğüm hizmeti kullanarak, ürününüzün altyapı yönünü merkezileştirirsiniz. Bu nedenle, merkeziyetsizliği son derecede önem veren projeler, üçüncü bir tarafa dış kaynak sağlamak yerine kendi kendini barındıran düğümleri tercih edebilir.

[Kendi düğümünüzü çalıştırmanın faydaları](/developers/docs/nodes-and-clients/#benefits-to-you) hakkında daha fazla bilgi edinin.

## Popüler düğüm hizmetleri {#popular-node-services}

İşte en popüler Ethereum düğüm sağlayıcılarından bazılarının bir listesi, eksik olanları eklemekten çekinmeyin! Her düğüm hizmeti, ücretsiz veya ücretli seviyelere ek olarak farklı avantajlar ve özellikler sunar, bir karar vermeden önce hangisinin ihtiyaçlarınıza en uygun olduğunu araştırmalısınız.

- [**Alchemy**](https://www.alchemy.com/)
  - [Belgeler](https://docs.alchemyapi.io/)
  - Özellikler
    - Ücretsiz seviye seçeneği
    - Kullandıkça ölçeklendirin
    - Ücretsiz arşiv verileri
    - Analiz araçları
    - Gösterge Paneli
    - Benzersiz API uç noktaları
    - Webkancaları
    - Doğrudan destek
- [**Ankr**](https://www.ankr.com/)
  - [Belgeler](https://docs.ankr.com/)
  - Özellikler
    - Ankr Protokolü - sekizden fazla zincirin Halka Açık RPC API uç noktalarına açık erişim
    - En yakındaki müsait düğüme hızlı ve güvenli bir geçit oluşturmak için yük dengeleme ve düğüm sağlığı takibi
    - WSS uç noktası ve sınırsız oran limitleri sağlayan Premium seviye
    - Kırktan fazla zincir için tek tıkla tam düğüm ve doğrulayıcı düğüm kurulumu
    - Kullandıkça ölçeklendirin
    - Analiz araçları
    - Gösterge Paneli
    - RPC, HTTPS ve WSS uç noktaları
    - Doğrudan destek
- [**BlockDaemon**](https://blockdaemon.com/)
  - [Belgeler](https://ubiquity.docs.blockdaemon.com/)
  - Faydalar
    - Gösterge Paneli
    - Düğüm bazında
    - Analizler
- [**Chainstack**](https://chainstack.com/)
  - [Belgeler](https://docs.chainstack.com/)
  - Özellikler
    - Ücretsiz paylaşılan düğümler
    - Paylaşılan arşiv düğümleri
    - GraphQL desteği
    - RPC ve WSS uç noktaları
    - Özel tam düğümler ve arşiv düğümleri
    - Özel dağıtımlar için hızlı eşitleme süresi
    - Bulutunuzu getirin
    - Saat başına ödeme fiyatlandırması
    - Doğrudan 7/24 destek
- [**GetBlock**](https://getblock.io/)
  - [Belgeler](https://getblock.io/docs/get-started/authentication-with-api-key/)
  - Özellikler
    - 40'tan fazla blok zinciri düğümüne erişim
    - 40 bin ücretsiz günlük talep
    - Sınırsız sayıda API anahtarı
    - 1 GB/sn ile yüksek bağlantı hızı
    - İzleme+Arşiv
    - Gelişmiş analizler
    - Otomatik güncellemeler
    - Teknik destek
- [**InfStones**](https://infstones.com/)
  - Özellikler
    - Ücretsiz seviye seçeneği
    - Kullandıkça ölçeklendirin
    - Analizler
    - Gösterge Paneli
    - Benzersiz API uç noktaları
    - Özel tam düğümler
    - Özel dağıtımlar için hızlı eşitleme süresi
    - Doğrudan 7/24 destek
    - 50'den fazla blok zinciri düğümüne erişim
- [**Infura**](https://infura.io/)
  - [Belgeler](https://infura.io/docs)
  - Özellikler
    - Ücretsiz seviye seçeneği
    - Kullandıkça ölçeklendirin
    - Ücretli arşiv verileri
    - Doğrudan Destek
    - Gösterge Paneli
- [**Kaleido**](https://kaleido.io/)
  - [Belgeler](https://docs.kaleido.io/)
  - Özellikler
    - Ücretsiz başlangıç ​​seviyesi
    - Tek tıklamayla Ethereum düğümü dağıtımı
    - Özelleştirilebilir istemciler ve algoritmalar (Geth, Quorum & Besu || PoA, IBFT & Raft)
    - 500+ yönetimsel ve servis API'leri
    - Ethereum işlem arzı için RESTful arayüz (Apache Kafka destekli)
    - Olay gönderimi için dışa yayınlar (Apache Kafka destekli)
    - Yan ve "zincir dışı" servislerin derin bir koleksiyonu (örneğin iki taraflı şifrelenmiş mesaj iletimi)
    - Yönetişimli ve rol esaslı erişim kontrollü açık ağ oryantasyonu
    - Hem yöneticiler hem uç kullanıcılar için çok yönlü kullanıcı yönetimi
    - Hayli ölçeklenebilir, esnek, hızlı ve güvenilir altyapı
    - Bulut HSM gizli anahtar yönetimi
    - Ethereum Mainnet Bağlama
    - ISO 27k ve SOC 2, Tip 2 sertifikasyonları
    - Dinamik program konfigürasyonu (örneğin bulut entegrasyonları ekleme, düğüm girdilerini değiştirme v.b.)
    - Çoklu bulut, çoklu bölge ve hibrit dağıtım düzenlemeleri için destek
    - Basit saatlik SaaS-esaslı ücretlendirme
    - SLA'lar ve 7/24 destek
- [**Moralis**](https://moralis.io/)
  - [Belgeler](https://docs.moralis.io/)
  - Özellikler
    - Ücretsiz paylaşımlı düğümler
    - Ücretsiz paylaşımlı arşiv düğümleri
    - Gizlilik odaklı (kayıt politikası yok)
    - Çapraz zincir desteği
    - Kullandıkça ölçeklendir
    - Gösterge Paneli
    - Benzersiz Ethereum SDK'si
    - Benzersiz API uç noktaları
    - Doğrudan teknik destek
- [**Pocket Network**](https://www.pokt.network/)
  - [Belgeler](https://docs.pokt.network/home/)
  - Özellikler
    - Merkeziyetsiz RPC Protokolü ve Pazar
    - Günlük 1 Milyon Talep Bulunan Ücretsiz Seviye (uç nokta başına maksimum 2)
    - [Açık Uç Noktalar](https://docs.pokt.network/home/resources/public-rpc-endpoints)
    - Pre-Stake+ Programı (günde 1 milyondan fazla isteğe ihtiyacınız varsa)
    - 15+ Blok Zinciri Desteklenir
    - Uygulamalara hizmet ederek POKT kazanan 6400+ Düğüm
    - Arşiv Düğümü, İzlemeli Arşiv Düğümü ve Test Ağı Düğümü Desteği
    - Ethereum Mainnet Düğüm İstemcisi Çeşitliliği
    - Tek Başarısızlık Noktası Yok
    - Sıfır Kesinti Süresi
    - Uygun Maliyetli Sıfıra Yakın Tokenomik (ağ bant genişliği için bir kez POKT stake edin)
    - Aylık batık maliyet yok, altyapınızı bir varlığa dönüştürün
    - Protokolde yerleşik olarak bulunan Yük Dengeleme
    - Gün başına talep sayısını ve saat başına düğüm sayısını sonsuz olarak ölçeklendirin
    - En özel, sansüre dayanıklı seçenek
    - Uygulamalı geliştirici desteği
    - [Pocket Portal](https://bit.ly/ETHorg_POKTportal) gösterge tablosu ve analizleri
- [**QuikNode**](https://www.quiknode.io/)
  - Özellikler
    - 7 günlük ücretsiz deneme
    - Çeşitli destek
    - Webkancaları
    - Gösterge Paneli
    - Analizler
- [**Rivet**](https://rivet.cloud/)
  - [Belgeler](https://rivet.readthedocs.io/en/latest/)
  - Özellikler
    - Ücretsiz seviye seçeneği
    - Kullandıkça ölçeklendirin
- [**SettleMint**](https://console.settlemint.com/)
  - [Belgeler](https://docs.settlemint.com/)
  - Özellikler
    - Ücretsiz deneme
    - Kullandıkça ölçeklendir
    - GraphQL desteği
    - RPC ve WSS uç noktaları
    - Özel tam düğümler
    - Bulutunuzu getirin
    - Analiz araçları
    - Gösterge Paneli
    - Saat başına ödeme fiyatlandırması
    - Doğrudan destek
- [**Watchdata**](https://watchdata.io/)
  - [Belgeler](https://docs.watchdata.io/)
  - Özellikler
    - Veri güvenilirliği
    - Kopmayan sıfır kesinti bağlantı
    - Süreç otomasyonu
    - Ücretsiz tarifeler
    - Tüm kullanıcılara uygun yüksek sınırlar
    - Çeşitli düğümler için destek
    - Kaynak ölçeklendirme
    - Yüksek işlem hızları

## Daha fazla bilgi {#further-reading}

- [Ethereum düğüm hizmetleri listesi](https://ethereumnodes.com/)

## İlgili konular {#related-topics}

- [Düğümler ve istemciler](/developers/docs/nodes-and-clients/)

## İlgili öğreticiler {#related-tutorials}

- [Alchemy kullanarak Ethereum geliştirmeye başlangıç](/developers/tutorials/getting-started-with-ethereum-development-using-alchemy/)
- [Web3 ve Alchemy kullanarak işlem gönderme kılavuzu](/developers/tutorials/sending-transactions-using-web3-and-alchemy/)

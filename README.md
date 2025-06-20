# Listing App 🚗📱

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Expo SDK](https://img.shields.io/badge/Expo%20SDK-53.0.9-blue)](https://expo.dev)
[![React Native](https://img.shields.io/badge/React%20Native-0.76.0-green)](https://reactnative.dev)
[![Strapi](https://img.shields.io/badge/Strapi-5-purple)](https://strapi.io)

**Listing App**, React Native ve Expo tabanlı, Vps sunucumdaki Strapi v5 backend ile entegre, sahibinden.com'u referans alan bir mobil uygulama. Kategoriler ve alt kategoriler arasında gezinme, ürün listeleme ve ilan oluşturma özellikleri sunar. NativeWind ile modern UI ve Expo Router ile akıcı navigasyon sağladım.

## 🎯 Özellikler

- **Dinamik Kategori ve Alt Kategori Listeleme**: Strapi API’sinden kategoriler (`/api/categories`) ve alt kategoriler (`/api/subcategories`) dinamik olarak çekilir.
- **Ürün Listeleme**: Kategori veya alt kategori bazında filtrelenmiş ürün listeleri.
- **İlan Oluşturma**: Kullanıcılar yeni ilan ekleyebilir (`PostAd`).
- **Kişiselleştirilmiş Öneriler**: Kullanıcıya özel içerik önerileri (`Personalized`).
- **Merkezi API Yönetimi**: Özel `useFetch` hook’u ile optimize edilmiş API çağrıları.
- **Modern UI**: NativeWind v4 ile Tailwind CSS tabanlı stil.
- **Akıcı Navigasyon**: Expo Router ile sekmeli navigasyon (ikinci sıradaki arama sekmesi, gizli tab bar).
- **Ikonlar**: Ionicons ile özelleştirilmiş kategori ve alt kategori ikonları.

## 🛠️ Teknoloji

| Teknoloji                 | Sürüm  | Açıklama                           |
| ------------------------- | ------ | ---------------------------------- |
| React Native              | 0.76.0 | Mobil uygulama çerçevesi           |
| Expo                      | 53.0.9 | Geliştirme ve dağıtım platformu    |
| NativeWind                | 4.1.23 | Tailwind CSS tabanlı stil          |
| Expo Router               | 5.0.7  | Dosya tabanlı navigasyon           |
| Strapi                    | 5.0.0  | Başsız CMS ve API backend          |
| React Native Vector Icons | 10.2.0 | Özelleştirilmiş ikonlar (Ionicons) |
| React                     | 19.0.0 | UI kütüphanesi                     |

## 📁 Dosya Yapısı

```bash
listing-app/
├── app/
│   ├── (tabs)/
│   │   ├── (search)/
│   │   │   ├── index.tsx            # Kategori listeleme ekranı
│   │   │   ├── _layout.tsx          # Arama uygulama düzeni
│   │   │   ├── subcategories.tsx    # Alt kategori listeleme
│   │   │   └── categoryproducts.tsx # Alt kategori ürün listeleme
│   │   ├── personalized.tsx         # Profil ekranı
│   │   ├── postad.tsx               # İlan oluşturma ekranı
│   │   ├── showcase.tsx             # Vitrin ekranı
│   │   ├── services.tsx             # Servisler ekranı
│   │   └── _layout.tsx              # Sekmeli navigasyon düzeni
│   ├── _layout.tsx                  # Genel uygulama düzeni
│   ├── login.tsx                    # Kullanıcı girişi ekranı
├── src/
│   ├── components/
│   │   ├── CustomHeader.tsx       # Özelleştirilmiş header
│   │   ├── ProductList.tsx        # Ürün listeleme
│   ├── hooks/
│   │   ├── useFetch.ts            # API için özel hook
│   │   └── useAuth.tsx            # Login için özel hook
├── assets/
│   ├── S-Logo1.png                # Logo
├── .env                           # VPS sunucumdaki Strapi api adresi (EXPO_PUBLIC_URL)
```

## 📸 Ekran Görüntüleri

| Showcase                                               | Search                                               | Post Ad                                            |
| ------------------------------------------------------ | ---------------------------------------------------- | -------------------------------------------------- |
| <img src="./assets/showcase-ekrani.png" width="300" /> | <img src="./assets/search-ekrani.png" width="300" /> | <img src="./assets/post-ekrani.png" width="300" /> |

| Services                                               | Personalized                                         | Login                                               |
| ------------------------------------------------------ | ---------------------------------------------------- | --------------------------------------------------- |
| <img src="./assets/services-ekrani.png" width="300" /> | <img src="./assets/profil-ekrani.png" width="300" /> | <img src="./assets/login-ekrani.png" width="300" /> |

| Car List                                               | Real Estate List                                               | Motocycles List                                               |
| ------------------------------------------------------ | -------------------------------------------------------------- | ------------------------------------------------------------- |
| <img src="./assets/car-list-ekrani.png" width="300" /> | <img src="./assets/real-estate-list-ekrani.png" width="300" /> | <img src="./assets/motocycles-list-ekrani.png" width="300" /> |

# Hukuk Botu

Bu proje, Llama-3-8B dil modeli ve RAG (Retrieval-Augmented Generation) mimarisi kullanılarak geliştirilmiş bir hukuk asistanıdır. Türk hukuku mevzuatına dayalı soruları yanıtlamak için vektör veritabanı kullanır.

## Özellikler

- **Model:** Unsloth ile optimize edilmiş Llama-3-8B-Instruct.
- **Veritabanı:** ChromaDB (Vektör veritabanı).
- **Yöntem:** RAG (Retrieval-Augmented Generation). Model, PDF formatındaki kanun kitaplarını tarayarak cevap üretir.

## Kurulum

Proje Google Colab üzerinde çalıştırılmak üzere tasarlanmıştır. Gerekli kütüphaneler not defteri içerisinde kurulmaktadır.

Gereksinimler:
- Python 3.10+
- GPU (Google Colab T4 önerilir)

Kütüphaneler:
`unsloth`, `langchain`, `chromadb`, `sentence-transformers`

## Kullanım

1. `hukuk.ipynb` dosyasını Google Colab'da açın.
2. Runtime türünü T4 GPU olarak ayarlayın.
3. Hücreleri sırasıyla çalıştırın.
4. `hukuk_asistani("sorunuz")` fonksiyonu ile test edebilirsiniz.

## Veri Seti

Model, RAG mimarisi için PDF formatındaki hukuk kitaplarını ve mevzuat metinlerini kullanır. Bu veriler vektörleştirilerek ChromaDB üzerinde tutulur.

## Lisans

MIT License

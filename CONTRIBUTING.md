# Katkıda Bulunma

_Kodsal bir katkıda bulunmak için lütfen README dosyasındaki Kurulum kısmını okuyun._

## Varolan Bir Jargonu Düzenleme

Varolan bir jargonu düzenlemek için ana dizinde bulunan `jargons` klasöründeki ilgili markdown dosyasını düzenleyip
pull request açabilirsiniz.

## Yeni Jargon Ekleme

Yeni jargon eklemek için ana dizinde bulunan `jargons` klasörü içinde yeni bir markdown dosyası oluşturun.

️️⚠️ **Dosya adı tamamen alfanümerik küçük harflerden oluşmalı ve boşluk yerine `-` karakteri kullanılmalıdır.**

Bu markdown dosyası içinde [frontmatter](https://jekyllrb.com/docs/frontmatter/) olarak aşağıdaki tablo oluşturulmalıdır.

| Ad       | Tip      | Zorunlu Mu | Açıklama                                                                                   |
| -------- | -------- | ---------- | ------------------------------------------------------------------------------------------ |
| title    | `string` | **evet**   | Jargon adı, tamamen küçük harflerle boşluklu veya Türkçe karakterler yazılabilir.          |
| sameWith | `array`  | **hayır**  | Aynı anlama gelen diger jargonlar. (Örnek: immutable için immutability)                    |
| tags     | `array`  | **hayır**  | Jargon etiketleri, tamamen küçük harflerle yazılmalıdır. En az bir tane olursa güzel olur. |

Markdown dosyasının geri kalan kısmında jargon ile ilgili açıklamalar yazılır. Açıklamada kullanılan başka jargon varsa bu
jargonlara link verilmesi güzel olur. Daha önce jargon.ist üzerinde tanımlanmamış bir jargon kullanımında onun için de
pull request açan contributor ise en güzel contributor 🚀👊'dır.

Tüm değişiklikler yapıldıktan sonra pull request açılır.

## Örnek bir Jargon dosyası

````md
---
title: jargon başlığı
sameWith:
- aynı anlama gelen başka bir jargon
tags:
- bir etiket
- bir başka etiket
---

Jargon ile ilgili **açıklama** satırları ve [baska jargon](/baska-jargona-link).

```js
function add(x, y) {
  return x + y;
}
```

Açıklamanın devami.
````
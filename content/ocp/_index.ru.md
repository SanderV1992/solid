+++
title = "OCP (Open Closed Principle)"
description = "OCP (Open Closed Principle)"
chapter = true
weight = 2
pre = "<b>2. </b>"
+++

## OCP (Open Closed Principle)
---
![ocp](ocp.jpg)
программные сущности (классы, модули, функции и т. п.) должны быть открыты для расширения, но закрыты для изменения.

#### Принцип OCP говорит о том что, программные сущности должны быть:
- открыты для расширения:
    это означает, что поведение модуля может быть расширено. Когда требования
    приложения изменяются, мы способны расширить модуль новыми линиями
    поведения, которые удовлетворяют возникшим изменениям.

    Другими словами, у нас есть возможность расширять классы, делая их более функциональными.
    При этом поведение старых методов не меняется, как и самого класса в целом.

- закрыты для изменения/модификации:
    в результате расширения поведения сущности,
    не должны вноситься изменения в код, который эти сущности использует.

---

#### Это особенно важно для боевого кода в производственной среде:
- любые изменения в исходном коде, требуют за собой пересмотр всего кода,
  где используется данная сущность/класс.

- пересмотр модульного тестирования и других подобных процедур.

Код, подчиняющийся данному принципу, не изменяется при расширении и поэтому не требует таких трудозатрат.

---
#### Read More:
- https://github.com/SanderV1992/SOLID-examples/tree/master/src/ocp/good
- <a href="https://ru.wikipedia.org/wiki/%D0%9F%D1%80%D0%B8%D0%BD%D1%86%D0%B8%D0%BF_%D0%BE%D1%82%D0%BA%D1%80%D1%8B%D1%82%D0%BE%D1%81%D1%82%D0%B8/%D0%B7%D0%B0%D0%BA%D1%80%D1%8B%D1%82%D0%BE%D1%81%D1%82%D0%B8">https://ru.wikipedia.org/</a>

### :warning: фасады не опредены

---

Для поддержки федеративного подхода к управлению архитектурой рекомендуется декларировать "фасады" -- объекты архитектуры, которые вы явным образом предлагаете к рассмотрению и переиспользованию в других доменах. 

Пример:

```yaml
# Первый способ
seaf.facades:                                                      
    - party_id
    - product_id                  

# Или второй способ
seaf.ba.parties:
    party_id:
        facade: true

seaf.ba.products:    
    product_id:
        facade: true
```

[Подробнее (facades_aliases.md)](/docs/seaf.ba.facades_aliases)
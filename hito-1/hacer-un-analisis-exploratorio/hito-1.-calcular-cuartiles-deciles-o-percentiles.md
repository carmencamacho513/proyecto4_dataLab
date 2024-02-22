---
description: BigQuery
---

# Hito 1. Calcular cuartiles, deciles o percentiles

```sql
SELECT
    APPROX_QUANTILES(DEP_TIME, 4) AS cuartiles_DEP_TIME,
    APPROX_QUANTILES(DEP_DELAY, 4) AS cuartiles_DEP_DELAY,
    APPROX_QUANTILES(ARR_DELAY, 4) AS cuartiles_ARR_DELAY,
    APPROX_QUANTILES(DELAY_DUE_CARRIER, 4) AS cuartiles_DELAY_DUE_CARRIER,
    APPROX_QUANTILES(DELAY_DUE_WEATHER, 4) AS cuartiles_DELAY_DUE_WEATHER,
    APPROX_QUANTILES(DELAY_DUE_NAS, 4) AS cuartiles_DELAY_DUE_NAS,
    APPROX_QUANTILES(DELAY_DUE_SECURITY, 4) AS cuartiles_DELAY_DUE_SECURITY,
    APPROX_QUANTILES(DELAY_DUE_LATE_AIRCRAFT, 4) AS cuartiles_DELAY_DUE_LATE_AIRCRAFT
  FROM
    `proyecto-4-datalab-413416.dataLab.imputados_202301`
```

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

Se realiza cuartiles en Big Query  para cada variable en estudio.

---
author: "Ilham N"
title: "Kamus Programmer 💻"
date: "2023-07-16"
description: "kumpulan kata/kalimat yang sering muncul ketika baca dokumentasi"
tags: ["web", "programmer", "book"]
draft: false
---

1. _imperative programming_ -> is like giving a chef step-by-step instructions on how to make a pizza.
2. _declarative programming_ -> is like ordering a pizza without being concerned about the steps it takes to make the pizza.
3. _circular dependency_
   Kamu punya dua file utama:

   env.config.ts → bertanggung jawab membaca .env, membuat config, dan menyiapkan httpsAgent, serta validasi.

   logger.ts → bertanggung jawab untuk mencatat log (log info, debug, warning, error).

   Keduanya saling berhubungan karena:

   logger.ts mengimpor config (untuk membaca app.debug).

   Kamu berencana membuat env.config.ts juga menggunakan Logger untuk mengganti console.log.

   Sehingga nanti terjadi saling impor dua arah:

   ```
   env.config.ts  --->  logger.ts
   logger.ts      --->  env.config.ts
   ```

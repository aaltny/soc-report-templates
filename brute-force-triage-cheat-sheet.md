# Brute-Force Triage — Cheat Sheet (1 Sayfa İskelet)

> Bu bir doldurma şablonudur. Her alert için kendi cümlelerinle doldur, kitaptan/TryHackMe'den metin kopyalama.

---

## Alert Bilgisi
- Tarih/Saat:
- Rule ID / Level:
- Rule Description:
- Agent (hostname / ID):

## Step 1 — Understand the Alert
*Bu alert ne söylüyor, hangi olay kaynağından geldi?*
-

## Step 2 — Identify Key Entities
- Kaynak IP:
- Hedef hesap:
- Hedef host:
- İlgili process/servis (varsa):

## Step 3 — Classify: Benign / Suspicious / Malicious
*İlk izlenim, sonraki adımlarda değişebilir.*
-

## Step 4 — Collect Supporting Evidence
- Deneme sayısı:
- Zaman aralığı (ilk-son olay):
- Başarılı giriş var mı? (4624 var mı):
- Aynı kaynaktan başka alert var mı:
- İlgili DQL sorguları:
  ```
  agent.id:XXX AND data.win.system.eventID:4625
  agent.id:XXX AND data.win.eventdata.targetUserName:"..."
  ```

## Step 5 — Determine Severity
*Gerçek ortam varsayımıyla düşün: hesap türü (admin mi?), başarı var mı, kaynak iç/dış mı.*
-

## Step 6 — Document Findings
*Kısa, olgusal, başkasının okuyup anlayabileceği şekilde yaz.*
-

## Step 7 — Escalate When Required
- Eskalasyon gerekli mi? (Evet/Hayır):
- Gerekçe:
- Kime / hangi süreçle:

---

## TP/FP Kararı
- [ ] True Positive
- [ ] False Positive
- Gerekçe:

## Hatırlatmalar
- Gerçek IP/hostname/parola yazma — `203.0.113.x` örnek aralığını kullan.
- Ekran görüntüsü alırken sansürlemeyi unutma.
- ATT&CK etiketini kör güvenme — Wazuh'un `rule.mitre` alanı yanlış olabilir, resmi sayfadan teyit et.

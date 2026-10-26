# Meetish · planlama mərhələsi

Bu qovluqda layihənin planlama mərhələsinin artifactları və birinci səhifənin ("Bu gün") dizaynı saxlanılır. Hələ kod yoxdur.

## Məzmun

| Qovluq | Nədir | Format |
|---|---|---|
| `01-planlama-senedi/` | İlk planlama araşdırması (faydalılıq, edge case-lər, rəqiblər, ideyalar, tech stack, dizayn və marketinq) | HTML (Claude Docs sənədinin HTML export-u, olduğu kimi) |
| `02-dizayn/canvas.json` | Dizayn kətanının quruluşu: lövhələrin yeri, adları və yanlarındakı qeydlər | JSON |
| `02-dizayn/boards/*.dc.html` | Kətandakı lövhələrin mənbə faylları: dizayn sistemi (`Main`), ilk "Bu gün" (`Home`), variantlar `BuGunA`–`BuGunE`, yekun `BuGunUI1` və `BuGunUI1Bubble` (avatar bubble) | HTML (artifactdan olduğu kimi) |
| `03-ui1-bu-gun/ui1-plan.xml` | "Bu gün" ekranının yekun planı: hər hissə hansı variantdan gəlib, qəbul olunmuş qaydalar, tokenlər, hələ çəkilməyənlər | XML |
| `03-ui1-bu-gun/preview/*.html` | `BuGunUI1` və `BuGunUI1Bubble` lövhələrinin brauzerdə birbaşa açılan nüsxəsi | HTML |

## Format haqqında

- Artifactların öz məzmunu HTML (XML-ə yaxın işarələmə) kimi dəyişdirilmədən saxlanılıb. Planlama sənədində yalnız müəllif qeydi daxili id-dən `@ilkin`-ə dəyişdirilib və səhifə `<html>` qabığına salınıb.
- `*.dc.html` faylları dizayn kətanının komponent formatıdır: `{{accent}}` kimi dəyişənlər və `support.js` kətanın öz runtime-ında işləyir, ona görə də bu fayllar brauzerdə tək açılanda tam görünmür. Baxmaq üçün `03-ui1-bu-gun/preview/` istifadə edin (accent `#D9431F` ilə doldurulub, lövhələr arası linklər söndürülüb).
- Qərarlar (ui1 planı) strukturlaşdırılmış XML kimi yazılıb ki, sonra kod və ya başqa alət tərəfindən oxunsun.

## Mənbələr (canlı versiyalar)

- Planlama sənədi: https://claude.ai/code/artifact/7bf895e8-0066-41c2-a456-76abd38287d6
- Android dizayn kətanı: https://claude.ai/artifact/5Lmh4QWA8sD33ZMtWt3dWy

Nüsxə tarixi: 2026-10-26. Kətandakı digər ekranlar (Sürətli plan, Plan detalı, Dostlar, Profil) birinci səhifəyə aid olmadığı üçün bura daxil edilməyib.

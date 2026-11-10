# Swipe file - Dubai real estate

آخر تحديث: 2026-11-10 (من /ig-viral، من 4 screenshots لتبويب الـ Reels)

```
SWIPE  ·  33 reels  ·  2 accounts  ·  baseline: account median
```

- **Account A** (وكيلة عقارات في دبي، screenshots 1-2): الـ median = **51,250**.
  اتحسب من 12 ريل مش متثبتين. استبعدت أحدث 3 ريلز (2,558 / 1,465 / 4,272) لأنهم شكلهم لسه نازلين وبيجمعوا مشاهدات.
- **Account B** (Springfield Properties، screenshots 3-4): الـ median = **26,900**، من 18 ريل.
- الـ handles مش ظاهرة في الـ screenshots، وافترضت إن كل اتنين screenshots حساب واحد.

## OUTLIERS (أكتر من 3x)

| multiple | views | account | الريل | formula |
| --- | --- | --- | --- | --- |
| 12.4x | 634,000 | A (pinned) | موقع فيلا تحت الإنشاء، مفيش كلام على الشاشة | مش معروف من غير ما نشوف الفيديو |
| 12.1x | 621,000 | A (pinned) | "INCOMING REACTION": رد على إسكتش "Realtors in 2026". أول سطر (مترجم): "عارفة إن ده إسكتش كوميدي، بس ممكن نكون صرحاء ثانية؟" | **Reaction / رد على كلام حد تاني** (مش موجود في hooks.json) |
| 4.1x | 208,000 | A (pinned) | "Dubai, 2008: I had just come back from Canada" | قصة بسنة ومكان، قريب من #21 Mid-Sentence |

التلاتة **pinned**، فممكن يكونوا قدام ومجمعين مشاهدات من شهور. الـ multiple بتاعهم غالباً أعلى من الحقيقي.

**Account B معندوش ولا outlier.** أعلى ريل 2.7x (72.4K، مشي قدام فيلا).
ريل "SO RAMIN PLEASE TELL ME" (ليه جزر دبي أحسن استثمار) جاب **0.7x**، يعني **أقل** من العادي بتاع الحساب.

## WHAT IS OVER-INDEXING

- **الريلز اللي فوق** واحد بيرد على كلام حد تاني، وواحد قصة شخصية بتاريخ، وواحد صورة مشروع حقيقي.
- **الريلز اللي تحت** معظمها لونشات وفعاليات ومشي في sales centers ("Pre Launch sales opening now"، "VIP Pre launch").
  دي كلها بين 0.5x و1x في الحسابين.
- **الإسكتشات والـ POV** ("When another agent steals your client"، "How government jobs work") بتجيب الأرقام العادية بتاعة الحساب، مش أكتر.

## UNCLASSIFIED

الـ 33 كلهم unclassified. الـ classifier بيقرا إنجليزي بس، ونص الريلز من غير كلام على الشاشة.
الشكل اللي يستاهل يتضاف لـ hooks.json: **الـ Reaction**. أول frame بيبقى كليب حد تاني (مشهور أو viral)،
وبعده بتوقفه وتقول الحقيقة اللي جوا المجال. ده الشكل اللي الـ skill اتوقع إنه ناقص
("a hook that opens on someone else's comment read out loud").

## CONFIDENCE

**ضعيفة.** 33 ريل من حسابين، والـ 3 outliers كلهم من حساب واحد ومتثبتين.
ده بيدي فكرة نجربها، مش نتيجة. محتاجين 6-10 حسابات وحوالي 12 ريل من كل واحد،
بالـ hook الحقيقي بالإنجليزي أو العربي زي ما اتقال، مش مترجم.

## YOUR VERSION

- **Reaction (الشكل الكسبان):** رد على ريل أو إعلان بيقول "عائد مضمون". الـ hook: "عائد مضمون {{X}}%؟ مضمون من مين؟"
  السكريبت الكامل اتكتب في /ig-viral بتاريخ 2026-11-10.
- **قصة بتاريخ (4.1x):** "{{السنة}}، {{أول صفقة / أول عقد قريته}}..." محتاج قصتك الحقيقية.

﻿# JavaScript-2

- Type Convirsions
- Operators
- Comparison
- Logical Operations ||&& !
- if else with multi condition
- if else with boolean condition
- order in if
- Nulish
- Differance beetween ?? and ||

Quyida siz so'ragan JavaScript mavzulari bo'yicha qisqa va aniq tushuntirishlar hamda amaliy misollar keltirilgan:

### 1. Type Conversions (Tiplarni o'zgartirish)
JavaScript-da qiymatlar avtomatik yoki qo'lda boshqa turdagi qiymatlarga o'zgartirilishi mumkin.

**Misollar:**
```javascript
let num = "123";  // String turidagi qiymat
let convertedNum = Number(num);  // Number turiga o'zgartirildi
console.log(convertedNum);  // 123
```

### 2. Operators (Operatorlar)
Operatorlar yordamida matematik yoki mantiqiy amallar bajariladi.

**Misollar:**
```javascript
let x = 10;
let y = 5;

console.log(x + y);  // Qo'shish operatori: 15
console.log(x - y);  // Ayirish operatori: 5
console.log(x * y);  // Ko'paytirish operatori: 50
console.log(x / y);  // Bo'lish operatori: 2
```

### 3. Comparison (Taqqoslash)
Taqqoslash operatorlari qiymatlarni solishtirish uchun ishlatiladi.

**Misollar:**
```javascript
let a = 10;
let b = "10";

console.log(a == b);  // true: qiymatlar teng (tiplarni tekshirmaydi)
console.log(a === b); // false: qiymatlar teng emas (tiplarni ham tekshiradi)
console.log(a != b);  // false: qiymatlar teng (tiplarni tekshirmaydi)
console.log(a !== b); // true: qiymatlar teng emas (tiplarni ham tekshiradi)
```

### 4. Logical Operations (`||`, `&&`, `!`) (Mantiqiy operatorlar)
Mantiqiy operatorlar yordamida shartlarni birlashtirish yoki ularning natijasini teskarisiga aylantirish mumkin.

**Misollar:**
```javascript
let isTrue = true;
let isFalse = false;

console.log(isTrue || isFalse);  // true: "yoki" operatori
console.log(isTrue && isFalse);  // false: "va" operatori
console.log(!isTrue);            // false: "emas" operatori
```

### 5. `if else` with Multi Condition (Ko'p shartli `if else`)
`if else` yordamida bir nechta shartlarni tekshirish mumkin.

**Misollar:**
```javascript
let age = 25;
let isStudent = false;

if (age > 18 && isStudent) {
  console.log("Siz talabasiz va yoshingiz 18 dan katta.");
} else if (age > 18) {
  console.log("Yoshingiz 18 dan katta, lekin siz talaba emassiz.");
} else {
  console.log("Yoshingiz 18 dan kichik.");
}
```

### 6. `if else` with Boolean Condition (`boolean` shartli `if else`)
`if` va `else` shartlari `boolean` qiymatlar asosida ishlaydi.

**Misollar:**
```javascript
let isLoggedIn = true;

if (isLoggedIn) {
  console.log("Xush kelibsiz!");
} else {
  console.log("Iltimos, tizimga kiring.");
}
```

### 7. Order in `if` (Shartlar ketma-ketligi)
`if else` ketma-ketligi bo'yicha shartlar yuqoridan pastga qarab tekshiriladi.

**Misollar:**
```javascript
let score = 85;

if (score >= 90) {
  console.log("A'lo baho.");
} else if (score >= 75) {
  console.log("Yaxshi baho.");
} else {
  console.log("Qoniqarli baho.");
}
```

### 8. Nullish Coalescing (`??`) Operatori
`??` operatori `null` yoki `undefined` bo'lgan qiymatlarni boshqa qiymatga almashtiradi.

**Misollar:**
```javascript
let name;
let displayName = name ?? "Ism yo'q";  // Agar `name` null yoki undefined bo'lsa, "Ism yo'q" ishlatiladi
console.log(displayName);  // "Ism yo'q"
```

### 9. Difference Between `??` and `||` (`??` va `||` farqi)
`||` operatori birinchi "truthy" (haqiqiy) qiymatni tanlaydi, `??` esa faqat `null` va `undefined` qiymatlarni tekshiradi.

**Misollar:**
```javascript
let emptyString = "";
let result1 = emptyString || "Noma'lum";  // Bo'sh string ham false bo'lgani uchun "Noma'lum" qaytadi
let result2 = emptyString ?? "Noma'lum";  // Bo'sh string truthy bo'lgani uchun "" qaytadi

console.log(result1);  // "Noma'lum"
console.log(result2);  // ""
```

Bu mavzular bo'yicha savollaringiz bo'lsa, qo'shimcha tushuntirishlar berishim mumkin.

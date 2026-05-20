BSV Montage Stundenkonto - kompletna aplikacija

ŠTA JE U PAKETU
1. React aplikacija za evidenciju sati
2. Supabase login i baza
3. Admin vidi sve sate/projekte/radnike
4. Radnik vidi samo svoje sate
5. PWA instalacija na telefon
6. CSV export

NAJVAŽNIJI FAJL ZA PROMJENE
src/config.js

Tu mijenjaš:
- companyName
- appName
- supabaseUrl
- supabaseAnonKey
- adminEmail

SUPABASE SETUP
1. Supabase Dashboard
2. SQL Editor
3. New Query
4. Otvori supabase/schema.sql
5. Sve kopiraj i klikni Run

ADMIN KORISNIK
1. U aplikaciji klikni “Novi korisnik”
2. Napravi korisnika sa emailom iz config.js, npr. simic@bsv-montage.de
3. U Supabase SQL Editor pokreni:
   update public.profiles set role = 'admin' where email = 'simic@bsv-montage.de';

LOKALNO TESTIRANJE
1. Instaliraj Node.js
2. Otvori terminal u folderu aplikacije
3. npm install
4. npm run dev

ONLINE
Najjednostavnije:
- uploaduj ovaj folder na GitHub
- poveži GitHub sa Vercel
- Vercel automatski deploy-a aplikaciju

TELEFON
Kad je aplikacija online:
Android Chrome: tri tačkice -> Install app
iPhone Safari: Share -> Add to Home Screen

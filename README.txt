TIMSS FREE HOSTING PACKAGE

النسخة مستقلة عن Lovable.

بعد النشر:
- رابط الطلاب: الصفحة الرئيسية.
- رابط الإدارة: نفس الرابط مع ?admin=results

قبل النشر:
1) ضع SUPABASE_URL و SUPABASE_ANON_KEY داخل index.html.
2) انشر Supabase Edge Function الموجودة في:
   supabase/functions/admin-results/index.ts
3) في Supabase Secrets عرّف:
   ADMIN_CODE
   SUPABASE_SERVICE_ROLE_KEY
4) يمكن نشر index.html مجانًا على GitHub Pages أو Cloudflare Pages.

النتائج تُحفظ مباشرة عبر anon key.
قراءة النتائج تتم فقط عبر Edge Function حتى لا ينكشف service role key في المتصفح.

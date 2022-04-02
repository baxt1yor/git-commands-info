$ git config --global user.name "#name" ||-> user name kiritish

$ git config --global user.email "#email" ||-> email kiritish

$ pwd ||-> mazkur papka manzili

$ git init ||-> mazkur papkani mahalliy talqinlar omborini sifatida belgilash

$ clear ||-> ekranni tozalash

$ git status ||-> o`zgarishlar bor yoki yo'qligini tekshirish

$ git status --untracked-files=all ||-> mahalliy talqinlar omboridagi barcha papkalardagi
o'zgarishlarni bor yoki yo`qligini tekshirish

$ git add #file_name ||-> faylni ro'yhatdan o'tkazish
 
$ git add . yoki * ||-> barcha fayllarni ro'yhatdan o'tkazish

$ git commit -m "#izoh" ||-> ro'yhatdan o'tgan fayllarni versiyalar (talqinlar)
omboriga o`zgarishlarni kuzatib borish uchun qo'shish

$ git commit -am "#izoh" ||-> ro'yhatdan o'tmagan fayllarni ro'yhatdan o'tkazish
va versiyalar omboriga qo'shish

$ git log ||-> versiyalar omboriga qo'shilgan barcha o'zgarishlarni ko'rish

$ git log --author="#author_name" ||-> biror avftorga tegishli bo'lgan o'zgartirishlar

$ git log --stat ||-> fayllardagi o'zgarishlar haqida ba'tafsil bilish

$ git log -2 ||-> oxirgi ikkitta o'zgarishni ko'rish

$ git log -2 --stat ||-> oxirgi ikkitta o'zgarishni ba'tafsil ko'rish

$ git log -p ||->talqinlar omboriga qo'shilgan fayllardagi o'zgartirishlarni
yanada ba'tafsilroq ko'rish

$ git diff ||-> hali ro'yhatdan o'tmagan o'zgarishlarni talqinlar omboriga qo'shilgan oxirgi
versiyasi bilan solishtirish/farqi

$ git diff --staged ||->ro'yhatdan o'tgan o'zgarishlarni talqinlar omboriga qo'shlgan oxirgi
versiyasi bilan solishtirish

$ git rm #file_name ||->faylni gitdan o'chirish

$ git checkout -- #file_name ||->o'zgartirilgan va ro'yhatdan o'tmagan faylni
ro'yhatdan o'tgan shakliga qaytarish

$ git reset HEAD #file_name ||->faylni ro'yhatdan chiqarish

$ git remote add origin https://github/.../ ||->mahalliy ombor bilan markaziy omborni ulash

$ git push -u origin master ||-> mahalliy ombordagi o'zgarishlarni markaziy omborga yuborish

$ git clone https://github/.../ ||->markaziy ombordan mahalliy omborga projectni klon qilib
olish

$ git pull origin master ||-> markaziy talqinlar omboridagi o`zgarishlarni mahalliy talqinlar
omboriga o'tkazish, markaziy ombordagi barcha o'zgarishlar mahalliy omborda paydo bo'ladi

$ git fetch ||-> markaziy talqinlar omboridagi o'zgarishlarni mahalliy talqinlar omboridagi
o'zgarishlar bilan solishtirish uchun olish, mahalliy ombordagi fayillar o`zgarishsiz qoladi

$ git diff master origin/master ||-> markaziy talqinlar omboridagi o'zgarishlarni mahalliy
versiyalar omboridagi o'zgarishlar bilan solishtirish/farqi

.gitignore ||-> ushbu formatdagi faylda kuzatilmasligi lozim bo'lgan har bir fayl yoki papka
nomlari alohida qatorga yoziladi
M:
fayl_nomi.formati            ||-> ushbu faylni kuztmaslik
papka_nomi                   ||->usbu papkani kuzatmaslik
papka_nomi/fayl_nomi.formati ||-> ushbu papkadagi mazkur faylni kuzatmaslik
*.txt                        ||-> txt formatdagi barcha fayllarni kuzatmaslik
papka_nomi/*.txt             ||-> ushbu papkadagi txt formatdagi barcha fayllarni kuzatmaslik
!test.txt                    ||-> ushbu faylni kuzatish(barcha fayllar kuzatmaslik uchun belgilaganda istesno fayllarni belgilash)


$ git branch ||->mahalliy talqinlar omboridagi barcha tarmoqlar

$ git brach #branch_name ||->yangi tarmoq hosil qilish

$ git checkout #branch_name ||->#branch_name ni asosiy tarmoq sifatida belgilash

$ git checkout -b #branch_name ||->yangi branch hosil qilish va shu branchni asosiy sifatida
belgilash

$ git branch -D #branch_name ||->branchni o'chirish

$ git merge #branch_name ||->aktiv tarmoqda va #branch_name dagi o`zgarishlarni hosil qilish,
aktiv tarmoqqa #branch_name ni birlashtirish

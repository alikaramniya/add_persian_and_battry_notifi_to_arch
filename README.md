# add_persian_and_battry_notifi_to_arch

#### برای اضافه کردن فونت فارسی کافیه دستور پایین رو توی ترمینال بزنید

```
sudo pacman -S ttf-dejavu ttf-liberation noto-fonts
```

#### حالا ی بار اگر سیستم رو reboot کنین همه چی حله


#### برای اضافه کردن نوتیفیکیشن هم میتونین از پکیج پایین استفاده کنین

```
cd ~
git clone https://aur.archlinux.org/i3-battery-popup-git.git
cd i3-battry-popup-git
makepkg -Acs
sudo pacman -U i3-battery-popup-git-r64.da5bcef-1-any.pkg.tar.zst
vim ~/.config/i3/config
```

#### بعد میری اخر فایل و کد پایین رو قرار میدی
```
exec --no-startup-id i3-battery-popu
```

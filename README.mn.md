# AI Box: серверийн суулгагч

AI Box-ийн төв серверийг (PC-A) Windows компьютер дээр суулгах файл, мөн суулгаж ашиглахыг алхам алхмаар
харуулсан богино видеонууд.

English: [README.md](README.md)

## Татах

- **Суулгагч:** [AIBox-HeadNode-Setup-Wizard.exe](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AIBox-HeadNode-Setup-Wizard.exe), хамгийн сүүлийн хувилбар.
  Бүх файл [Releases](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest) хуудсанд байна.
- **Заавар видео:**
  1. [Сервер суулгах](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AI-Box-guide-1-server-setup.mp4) (3:29)
  2. [Ажилтны компьютерт суулгах, файл хуваалцах](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AI-Box-guide-2-employee-computer.mp4) (3:08)
  3. [Windows анхааруулбал](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AI-Box-guide-3-windows-warnings.mp4) (2:47)
  4. [AI Box вэб хуудсыг ашиглах](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AI-Box-guide-4-web-page.mp4) (3:47)

## Сервер болох компьютерт хэрэгтэй

Windows 10 22H2 эсвэл 11, 8 GB санах ой, 10 GB сул зай, интернет, администраторын эрх. Компьютер асаалттай,
цахилгаанд залгаатай байна: бусад компьютер AI Box-т үүгээр холбогдоно.

## Суулгах

1. Файлыг давхар дарна. «Windows protected your PC» гарвал **More info → Run anyway** (суулгагч гарын үсэггүй),
   өөрчлөлт хийхийг зөвшөөрөх эсэхийг асуухад **Yes**.
2. Хэлээ сонгоод (англи эсвэл монгол) алхмуудыг дагана: 10–20 минут, нэг удаа дахин асааж магадгүй.
3. Сүүлийн хуудсанд гарах вэб хаяг, нууц үгсийг хадгална: дахин харагдахгүй.
4. Ажилтны компьютерт: суулгагч `C:\AIBox\AIBox-Agent-Setup.exe`-г үүсгэнэ. Үүнийг компьютер бүр дээр хуулж
   ажиллуулна. Энэ файл таны серверт нэвтрэх түлхүүртэй тул нийтэд бүү тарааж байгаарай.

## Файлыг шалгах

PowerShell дээр, файл байгаа хавтсанд:

```powershell
Get-FileHash .\AIBox-HeadNode-Setup-Wizard.exe
```

Гарсан *Hash* нь release-ийн тэмдэглэл дэх SHA-256-тай яг ижил байх ёстой.

## Docker Desktop

Сервер Docker Desktop дээр ажиллана. 250-аас олон ажилтантай, эсвэл жилийн орлого нь 10 сая ам.доллараас дээш
байгууллагад Docker-ийн төлбөртэй захиалга хэрэгтэй.

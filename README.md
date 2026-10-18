# AI Box: серверийн суулгагч

AI Box-ийн төв серверийг (PC-A) Windows компьютер дээр суулгах файл.

**Татах:** [AIBox-HeadNode-Setup-Wizard.exe](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AIBox-HeadNode-Setup-Wizard.exe)
(хамгийн сүүлийн хувилбар: [Releases](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest)).

**Шаардлага:** Windows 10 22H2 эсвэл 11, 8 GB санах ой, 10 GB сул зай, интернет, администраторын эрх. Сервер
болох компьютер асаалттай, цахилгаанд залгаатай байна.

1. Файлыг давхар дарна. «Windows protected your PC» гарвал **More info → Run anyway** (суулгагч гарын үсэггүй),
   «Allow changes?» → **Yes**.
2. Хэлээ сонгоод алхмуудыг дагана: 10–20 минут, нэг удаа дахин асааж магадгүй.
3. Сүүлийн хуудсанд гарах вэб хаяг, нууц үгсийг хадгална: дахин харагдахгүй.
4. Ажилтны компьютерт: суулгагч `C:\AIBox\AIBox-Agent-Setup.exe`-г үүсгэнэ. Үүнийг компьютер бүр дээр хуулж
   ажиллуулна. Энэ файл таны серверт нэвтрэх түлхүүртэй тул нийтэд бүү тарааж байгаарай.

**Файлыг шалгах:** PowerShell дээр `Get-FileHash .\AIBox-HeadNode-Setup-Wizard.exe`: гарсан Hash нь release-ийн
тэмдэглэл дэх SHA-256-тай яг ижил байх ёстой.

**Docker Desktop:** сервер Docker Desktop дээр ажиллана. 250-аас олон ажилтантай, эсвэл жилийн орлого нь $10M-аас
дээш байгууллагад Docker-ийн төлбөртэй захиалга хэрэгтэй.

---

**English.** The installer for the AI Box server (PC-A) on Windows. Download the latest release and run it
(*More info → Run anyway*: it is not signed; then *Yes*), follow the wizard (10–20 minutes), and keep the address and
passwords its last page shows. It creates `C:\AIBox\AIBox-Agent-Setup.exe` for the employees' computers: it carries a
key to your server, so do not share it publicly. Needs Windows 10 22H2 or 11, 8 GB of memory, 10 GB free, internet
and an administrator. Check the download with `Get-FileHash`: the SHA-256 is in the release notes. The server runs
on Docker Desktop, whose terms ask organizations above 250 employees or $10M a year for a paid subscription.

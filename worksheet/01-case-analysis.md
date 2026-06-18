---
artifact: 01 - Case Analysis
bai-tap: Lab 1 - Phan tich "tu huyet" chien luoc
format: Ca nhan truoc -> share trong ban -> chot verdict cuoi
time: 20 phut tren lop
nop-cuoi: Co - day la file nop cuoi cua Lab 1
---

# Lab 1 - Case Analysis / Phan tich "tu huyet" chien luoc

**Case da chon:** FPT Software / FPT Corporation - mo hinh outsource phan mem bi re-rating boi AI coding  
**Nguoi lam:** Nguyen Van Duong  
**Ban / nhom ban:** 
**Ngay:** 18/06/2026

## Buoc 0 - Chon case that nhanh

- **Case / san pham / cong ty:** FPT Software, mang dich vu CNTT va outsource phan mem cua FPT Corporation.
- **AI / platform / san pham moi tao ap luc:** GitHub Copilot, ChatGPT, Claude/Cursor va cac agent coding co kha nang tao code, test, debug, viet tai lieu.
- **Vi sao toi chon case nay?**  
  > FPT tung duoc thi truong dinh gia nhu mot cong ty cong nghe tang truong cao nho loi the nhan luc ky su, nang luc delivery offshore va khach hang quoc te. AI khong "giet" FPT ngay, nhung lam thay doi cach khach hang mua dich vu outsource: ho khong chi mua gio cong lap trinh nua, ma doi hoi nang suat, outcome va nang luc AI-native.

## Buoc 1 - Gom 3-5 bang chung chot

| # | Bang chung / so lieu chot | Vi sao so nay quan trong? | Nguon |
|---|---|---|---|
| E1 | FPT Software la nha cung cap dich vu CNTT/toan cau va outsource phan mem, co mat tai hon 30 quoc gia, hon 80 van phong, khoang 30.000 nhan su; doanh thu Global IT Services da vuot moc 1 ty USD nam 2023. | Cho thay "case truoc AI" cua FPT dua nhieu vao quy mo nhan luc, delivery offshore va kha nang ban dich vu phan mem cho khach hang quoc te. | FPT Software overview: https://en.wikipedia.org/wiki/FPT_Software |
| E2 | Nam 2024, FPT/FPT Software tiep tuc bao cao tang truong manh, doanh thu 2024 khoang 2,47 ty USD va loi nhuan truoc thue khoang 434,57 trieu USD; cung nam do FPT xay 2 AI Factories tai Viet Nam va Nhat Ban voi NVIDIA. | Day la bang chung hai mat: FPT van la cong ty tot, nhung ban than FPT cung phai chuyen sang AI infrastructure/AI service de tranh bi commoditize. | FPT Corporation / FPT Software summaries: https://en.wikipedia.org/wiki/FPT_Corporation |
| E3 | Nghien cuu ve GitHub Copilot cho thay lap trinh vien hoan thanh tac vu nhanh hon 55,8% trong thi nghiem co kiem soat. | Neu AI lam tang nang suat lap trinh, khach hang outsource se hoi lai: vi sao van tra tien theo so nguoi/so gio nhu cu? | "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot": https://arxiv.org/abs/2302.06590 |
| E4 | Stack Overflow Developer Survey 2025 duoc bao cao la 84% developer dang dung hoac du dinh dung AI tools; tuy nhien 46% khong tin do chinh xac cua output AI. | AI da vao workflow dai tra, nhung chua thay the hoan toan con nguoi. Loi the moi khong phai "co nhieu coder" ma la "biet ket hop AI + governance + domain expertise". | ITPro tong hop Stack Overflow Survey 2025: https://www.itpro.com/software/development/developers-arent-quite-ready-to-place-their-trust-in-ai-nearly-half-say-they-dont-trust-the-accuracy-of-outputs-and-end-up-wasting-time-debugging-code |
| E5 | Gia co phieu FPT tren HOSE co giai doan giam dang ke sau vung dinh 2024/2025; toi xem day la tin hieu thi truong dang chiet khau lai ky vong tang truong/dinh gia, trong do AI la mot rui ro chien luoc lon voi mo hinh outsource. | Gia co phieu khong chung minh AI la nguyen nhan duy nhat, nhung la dau hieu nha dau tu bat dau hoi: tang truong nhan luc va billable hours con ben vung khong khi AI lam giam gia tri coding commodity? | Bieu do HOSE:FPT tren TradingView/SSI/iBoard hoac trang chung khoan dang dung khi nop bai. |

### 3 phat hien ban dau

1. **Case nay tung thang nho...**  
   > kha nang tuyen, dao tao va quan tri so luong lon ky su phan mem voi chi phi canh tranh, cong voi nang luc delivery cho khach hang Nhat, My, chau Au.
2. **AI shock lam thay doi...**  
   > don vi gia tri trong outsource: tu "so gio lap trinh/so nguoi trong team" sang "toc do ra output, chat luong, IP, domain knowledge va trach nhiem ket qua".
3. **Dau hieu manh nhat cho thay luat choi moi la...**  
   > AI coding tools da vao workflow dai tra, FPT cung phai dau tu AI Factory/NVIDIA; nghia la day khong con la xu huong ben le ma la nen tang canh tranh moi.

## Buoc 2 - Viet 4 nhan dinh bat buoc

### Nhan dinh 1 - Truoc AI, case nay thang nho gia dinh gi?

**Tra loi cua toi:**  
> Truoc AI, FPT Software thang nho gia dinh rang khach hang quoc te can "thue nang luc lap trinh ben ngoai" voi chi phi thap hon, quy mo linh hoat hon va delivery on-time hon so voi tu xay team noi bo. Gia tri loi cua FPT la quy mo ky su, process delivery, quan he khach hang, nang luc tieng Nhat/thi truong Nhat va kha nang chay du an lon.
>
> Job-to-be-done ma khach hang "thue" FPT lam la: bien nhu cau so hoa/phan mem thanh he thong chay duoc ma khong phai tu tuyen, dao tao va quan tri toan bo doi ngu ky thuat.

**Bang chung do nhan dinh nay:** E1, E2

### Nhan dinh 2 - Ky vong nguoi dung va luat choi canh tranh da doi o dau?

**Shift ky vong quan trong nhat:** Lam xong giup toi / tra theo ket qua  
**Competitive dynamic quan trong nhat:** switching costs giam va build-copy cycles tang toc

**Tra loi cua toi:**  
> Khach hang outsource khong con mac dinh chap nhan viec tang headcount la cach chinh de tang output. Khi Copilot/ChatGPT/Claude co the tao code, test, refactor, viet tai lieu nhanh hon, buyer se ky vong nha cung cap dich vu phai dung AI de giao nhanh hon, it nguoi hon, minh bach hon va gan voi business outcome hon.
>
> Luat choi canh tranh doi tu "ai co nhieu ky su hon" sang "ai co workflow AI-native, data/domain context, quality gate va governance tot hon". Neu FPT chi ban manpower, phan gia tri do de bi ep gia; neu FPT ban AI-enabled delivery va domain solution, FPT van co cua song.

**Bang chung do nhan dinh nay:** E3, E4, E5

### Nhan dinh 3 - Gia dinh nao khong con dung nua? Dieu gi da thay doi vinh vien?

**Dieu da thay doi vinh vien theo toi la:**  
> Gia dinh "lap trinh vien la don vi san xuat chinh va gio cong la don vi tinh tien tu nhien" khong con chac dung. AI bien mot phan coding, test, debug, document thanh cong viec co the tu dong hoa hoac tang toc manh. Tu day, khach hang se ngay cang hoi ve gia tri cuoi cung: thoi gian ra san pham, chat luong, bao mat, hieu biet domain va kha nang chiu trach nhiem.
>
> Phan khuc outsource van ton tai, nhung cach phuc vu se khac: it giong "cho thue coder" va giong "doi tac delivery co AI, co tai san tai su dung, co chuyen mon nganh" hon. Dieu vinh vien khong phai la gia FPT giam, ma la chuan moi trong dau buyer: nha cung cap phan mem phai chung minh nang suat AI va outcome.

**Bang chung do nhan dinh nay:** E3, E4, E5

### Nhan dinh 4 - Case nay con cuu duoc khong? Neu co, phai doi bang cach nao?

**Verdict ban dau cua toi:** Co nhung phai doi rat manh

**Tra loi cua toi:**  
> FPT khong phai case "chet vi AI"; day la case "bi AI buoc phai doi moat". FPT con nhieu loi the: khach hang lon, uy tin delivery, thi truong Nhat, quy mo nhan luc, FPT Education va kha nang dau tu ha tang AI. Nhung neu FPT tiep tuc de thi truong nhin minh nhu cong ty outsourcing theo billable headcount, valuation se bi ep.
>
> Cach doi la chuyen tu labor arbitrage sang AI-native service: dung AI de tang nang suat noi bo, dong goi solution theo nganh, ban outcome/SLA thay vi chi ban so nguoi, xay governance bao mat cho enterprise, va bien AI Factory thanh nang luc giao hang that chu khong chi la cau chuyen truyen thong.

**Bang chung do nhan dinh nay:** E2, E3, E4

## Tom tat ca nhan truoc khi share trong ban

1. `Case nay yeu di vi...` FPT Software neu chi duoc nhin nhu nha cung cap gio cong lap trinh se bi AI coding tools lam giam gia tri cua phan coding commodity.
2. `Dieu thay doi vinh vien la...` buyer outsource se doi hoi nang suat AI, delivery theo outcome va domain expertise, khong con mac dinh tra tien theo headcount.
3. `Verdict cua toi la...` FPT con cuu duoc, nhung phai doi tu labor outsourcing sang AI-native delivery partner.

## Buoc 3 - Share trong ban

| Nguoi | Case | Bang chung manh nhat ho neu | Dieu ho cho la "thay doi vinh vien" | Verdict cua ho |
|---|---|---|---|---|
| Ban 1 | Chegg | Thue bao giam manh sau ChatGPT | Entry point hoc tap chuyen sang chatbot | Kho cuu neu chi ban loi giai |
| Ban 2 | Stack Overflow | Developer hoi AI thay vi len forum | Knowledge Q&A bi AI chen vao workflow | Phai thanh data/enterprise layer |
| Ban 3 | FPT outsourcing | AI coding tang nang suat va FPT phai dau tu AI Factory | Billable headcount khong con la moat du | Co nhung phai doi manh |
| Ban 4 | Jasper | Copywriting generic bi ChatGPT ep gia | Lop vo prompt/content de bi commoditize | Phai di vao workflow marketing sau hon |

**1. Ban toi thay case nao co bang chung manh nhat? Vi sao?**  
> Chegg va Stack Overflow co bang chung tac dong truc tiep hon ve user/traffic. Case FPT kho hon vi gia co phieu chi la tin hieu gian tiep, nhung no dang gia tri vi cho thay AI anh huong ca nhung cong ty van tang truong tot.

**2. Co pattern nao lap lai giua nhieu case khong?**  
> Pattern lap lai la AI chiem entry point va lam giam gia tri cua tac vu generic. Noi nao san pham chi ban "lam ho mot viec co the prompt ra duoc", switching cost giam rat nhanh. Noi nao co du lieu rieng, workflow sau, trust va accountability thi con loi the.

**3. Mot canh bao cho chinh du an cua nhom toi la gi?**  
> Dung xay san pham chi la lop vo mong tren AI. Phai chon mot workflow co pain that, co du lieu/ngu canh rieng va co ly do de user tin ket qua hon viec tu hoi ChatGPT.

## Buoc 4 - Chot lai verdict ca nhan sau thao luan

### Sau khi nghe ban phan bien, verdict cua toi:

- [ ] Giu nguyen
- [x] Doi nhe
- [ ] Doi manh

### Vi sao toi giu / doi verdict?

> Toi doi nhe vi ban gop y rang khong nen viet "gia co phieu FPT giam boi AI" nhu mot quan he nhan qua chac chan. Cach viet dung hon la: AI la mot rui ro chien luoc lam thi truong re-rating cac cong ty outsourcing; gia co phieu la mot tin hieu, khong phai bang chung duy nhat.
>
> Vi vay verdict cuoi tap trung vao thay doi vinh vien trong buyer expectation, khong tap trung vao bien dong gia ngan han.

### Verdict cuoi cung cua toi (phien ban nop)

**Case nay ton thuong truoc AI vi:**  
> Mot phan gia tri cua FPT Software nam o viec cung cap ky su va gio cong phan mem quy mo lon. AI coding tools lam phan viec coding/test/document generic nhanh hon va re hon, khien khach hang outsource co ly do ep gia hoac doi hoi output cao hon voi it nguoi hon.

**Dieu thay doi vinh vien la:**  
> Trong dich vu phan mem, "nhieu lap trinh vien" khong con tu dong dong nghia voi "nhieu gia tri". Chuan moi la AI-native delivery: nhanh hon, co domain context, co quality/security governance va gan voi outcome kinh doanh.

**Neu phai rut 1 bai hoc cho du an cua nhom minh, toi rut ra:**  
> Dung xay AI product dua tren tac vu generic de bi copy. Phai tim dung job dau nhat trong workflow, gan AI vao noi tao outcome ro, va co mot moat ngoai model nhu du lieu rieng, quy trinh tin cay, domain expertise hoac distribution.

## Checklist truoc khi nop

- [x] Toi da chon it nhat 3 bang chung chot co nguon.
- [x] Moi nhan dinh deu chi vao it nhat 1 bang chung.
- [x] Toi da ghi lai phan share trong ban.
- [x] Toi da viet verdict cuoi sau thao luan.


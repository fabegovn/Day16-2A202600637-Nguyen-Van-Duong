---
artifact: 02 - JTBD Project Analysis
bai-tap: Lab 2 - Dung JTBD de soi lai du an nhom
format: Theo nhom du an -> share trong ban -> chot hypothesis cuoi
time: 25 phut tren lop
nop-cuoi: Co - day la file nop cuoi cua Lab 2
companion-reference: Strategyn_JTBD_Playbook.pdf
---

# Lab 2 - JTBD Project Analysis / Dung JTBD de soi lai du an nhom

**Ten du an / san pham:** AI Delivery Copilot cho team outsource phan mem

## Buoc 0 - Khoanh dung 1 lat cat cua du an

- **Du an cua nhom toi la:** AI Delivery Copilot giup team outsource phan mem bien yeu cau khach hang thanh plan, task, test case va bao cao tien do co kiem soat.
- **Lat cat toi chon de phan tich hom nay la:** Giup Project Manager / Tech Lead trong cong ty outsource xu ly yeu cau moi tu khach hang enterprise truoc khi giao cho developer.
- **Vi sao toi chon lat cat nay:**  
  > Day la diem dau va co tac dong lon: neu hieu sai requirement, toan bo sprint bi tre, estimate sai, dev lam lai nhieu va khach hang mat tin tuong.

## Buoc 1 - Project Snapshot

1. **Nhom toi dang nghi minh dang giai quyet van de gi?**  
   > Team outsource ton nhieu thoi gian doc requirement, hoi lai khach hang, tach task, estimate, viet acceptance criteria va cap nhat tien do.

2. **Nguoi dung chinh hien nhom dang nham toi la ai?**  
   > Project Manager / Tech Lead phu trach mot team outsource 5-20 developer.

3. **Hien tai nguoi dung do dang giai quyet van de nay bang cach nao?**  
   > Doc tai lieu khach hang thu cong, hop voi BA/dev, viet ticket tren Jira, dung template Excel/Google Docs, hoi ChatGPT rieng le va tu kiem tra lai.

## Buoc 2 - Market Context

1. **Ai dang gap van de nay?**  
   > PM/Tech Lead trong cong ty outsource phan mem lam du an cho khach hang quoc te.

2. **Van de xuat hien trong hoan canh nao?**  
   > Khi khach hang gui requirement moi, change request hoac feedback gap truoc sprint planning.

3. **Hien tai ho dang dung giai phap thay the nao?**  
   > Jira, Confluence, Excel, Google Docs, hop noi bo, ChatGPT/Copilot dung ca nhan, va kinh nghiem cua senior.

4. **Vi sao day la thoi diem dang giai?**  
   > AI coding lam khach hang ky vong delivery nhanh hon, nhung bottleneck thuc te chuyen len buoc hieu dung requirement, tach viec va kiem soat chat luong.

### Tom tat market context

> Outsource phan mem khong chi can viet code nhanh; can bien yeu cau mo ho cua khach hang thanh cong viec ro, co uu tien, co acceptance criteria va co risk tracking.  
> Khi AI lam coding nhanh hon, loi the cua nha cung cap dich vu nam o kha nang dieu phoi workflow, domain context va dam bao chat luong.  
> Neu PM/Tech Lead van lam buoc phan tich requirement thu cong, team se khong tan dung duoc AI va van bi tre o dau sprint.

## Buoc 3 - Job Executor

- **Job executor cua du an nay la:** Project Manager / Tech Lead trong team outsource phan mem.
- **Vi sao toi tin day la nguoi truc tiep "thue" giai phap de lam job:**  
  > Ho la nguoi nhan requirement, quyet dinh cach tach task, hoi lai khach hang, phan cong dev va chiu trach nhiem khi sprint tre hoac deliver sai.

## Buoc 4 - Core JTBD

**Core JTBD ban nhap:**  
> Bien requirement cua khach hang thanh ke hoach delivery ro rang bang AI.

**Cac tu solution toi dang lo nhet vao cau:** AI

**Core JTBD cuoi cung:**  
> Chuyen yeu cau khach hang thanh ke hoach delivery ro rang, co the giao viec va kiem soat duoc truoc khi sprint bat dau.

## Buoc 5 - 3 Job Stories

| # | Trigger / When | Motivation / I want to | Outcome / so I can | Dieu story nay cho thay |
|---|---|---|---|---|
| JS1 | When khach hang gui requirement moi bang email/tai lieu dai | I want to tom tat scope, cau hoi mo va rui ro chinh | so I can phan hoi nhanh ma khong bo sot diem quan trong | Pain nam o buoc doc-hieu va clarify requirement |
| JS2 | When sprint planning sap dien ra nhung requirement con mo ho | I want to tach thanh epic/story/task kem acceptance criteria | so I can giao viec cho dev va QA ma it phai lam lai | Pain nam o prepare/confirm truoc khi execute |
| JS3 | When khach hang thay doi scope giua sprint | I want to thay tac dong len timeline, task va risk | so I can thuong luong lai deadline/effort co co so | Pain nam o modify va monitor change |

## Buoc 6 - Current Alternatives

| Alternative hien tai | User dang thue no de lam gi? | No lam tot gi? | No fail o dau? | Switching cost hien tai cao hay thap? |
|---|---|---|---|---|
| Jira + Confluence | Ghi task, tai lieu, trang thai | Chuan enterprise, team quen dung | Khong tu hieu requirement, khong tu tao cau hoi/risk | Cao vi da nam trong workflow |
| Hop noi bo voi BA/dev senior | Lam ro scope va estimate | Co context va judgement nguoi that | Ton thoi gian, phu thuoc senior, kho scale | Trung binh |
| ChatGPT/Copilot ca nhan | Tom tat, viet draft ticket/test case | Nhanh, re, linh hoat | Roi rac, kho bao mat, khong gan voi Jira/context du an | Thap |

**Neu project cua toi bien mat hom nay, user nhieu kha nang se quay ve:**  
> Jira/Confluence + hop noi bo + dung ChatGPT rieng le de tao draft.

## Buoc 7 - JTBD Lite Map

| Step | Trong workflow nay user dang co lam gi? | Hom nay ho dang dung gi? | Friction / pain hien tai | Muc dau |
|---|---|---|---|---|
| Define | Xac dinh muc tieu, scope, deadline, stakeholder | Email, brief, hop kickoff | Requirement dai, mo ho, nhieu assumption an | High |
| Locate | Tim tai lieu, API, ticket cu, decision cu | Confluence, Drive, Jira | Context nam rai rac nhieu noi | Med |
| Prepare | Tach epic/story/task, viet AC, estimate | Jira, Excel, hop team | Ton thoi gian, chat luong phu thuoc senior | High |
| Confirm | Hoi lai khach hang, chot scope va acceptance | Email, meeting notes | Cau hoi khong day du, de miss edge case | High |
| Execute | Dev code, QA test | IDE, GitHub, CI/CD, Copilot | AI ho tro code nhung neu task sai thi van lam lai | Med |
| Monitor | Theo doi tien do, blocker, scope creep | Jira dashboard, daily standup | Bao cao tre, risk phat hien muon | Med |
| Modify | Xu ly change request giua sprint | Hop gap, sua ticket thu cong | Kho thay tac dong len timeline/effort | High |
| Conclude | Tong ket delivery, demo, lesson learned | Report, retrospective | Knowledge khong duoc tai su dung tot | Low |

**Buoc dau nhat #1:** Prepare  
**Buoc dau nhat #2:** Confirm

**Vi sao day la noi dang chu y nhat:**  
> Neu prepare/confirm sai, AI coding o buoc execute chi giup team lam nhanh mot viec sai.  
> Day cung la noi PM/Tech Lead co nhieu tai lieu, ngu canh va quy tac de AI ho tro, nhung van can nguoi chot de tranh sai requirement.

## Buoc 8 - AI Leverage Point

| Step | AI nen giup bang cach nao? | Vi sao AI hop o day? | Rui ro chinh neu dung AI |
|---|---|---|---|
| Prepare | Doc requirement, de xuat epic/story/task, acceptance criteria, test ideas va estimate range | Day la tac vu nhieu ngon ngu tu nhien, co pattern lap lai, can draft nhanh | Hallucinate scope, estimate ao, bo sot rui ro domain |
| Confirm | Tao danh sach cau hoi clarify, risk log va impact neu khong chot | AI gioi trong viec soat lo hong va doi chieu checklist | Hoi qua nhieu cau chung chung, lam khach hang roi |

**AI leverage point quan trong nhat cua du an toi la:**  
> Bien requirement mo ho thanh draft backlog + cau hoi clarify + risk log truoc sprint planning.

**Vi sao khong phai o buoc khac:**  
> Execute da co Copilot/Cursor ho tro code. Pain lon hon nam truoc khi code: hieu sai, tach sai, confirm thieu. Neu chen AI vao prepare/confirm, team giam rework va tang do tin cua delivery.

## Buoc 9 - Product Hypothesis

> Neu chung ta giup PM/Tech Lead chuyen yeu cau khach hang thanh backlog, acceptance criteria va cau hoi clarify tot hon o buoc Prepare/Confirm,  
> bang cach dung AI doc requirement, truy xuat context du an va de xuat risk/task co human approval,  
> thi ho se chuyen tu Jira + hop thu cong + ChatGPT rieng le sang AI Delivery Copilot tich hop voi workflow du an,  
> vi ho tiet kiem thoi gian planning, giam rework va co bang chung ro hon khi thuong luong scope voi khach hang.

### Tin hieu som neu hypothesis nay dung

1. PM/Tech Lead san sang dua requirement that vao tool va dung draft ticket trong sprint planning.
2. Thoi gian tu luc nhan requirement den luc co backlog draft/cau hoi clarify giam it nhat 30%.

## Buoc 10 - Assumptions to Validate

| Assumption | Vi sao assumption nay rui ro? | Toi dang co bang chung gi? | Can validate bang cach nao tiep theo? |
|---|---|---|---|
| A1: PM/Tech Lead la job executor dung | Neu BA moi la nguoi lam chinh, product se sai user | Suy luan tu workflow outsource | Phong van 5 PM/Tech Lead va 5 BA |
| A2: Prepare/Confirm la pain du dau | Neu pain that nam o sales/contract hoac QA, leverage point sai | Logic tu rework trong sprint | Diary study 2 sprint, do thoi gian planning/rework |
| A3: User tin AI neu co human approval | Neu AI bi xem la qua rui ro, adoption thap | AI hien da duoc dung ca nhan | Prototype voi audit trail va approval flow |
| A4: Tich hop Jira/Confluence du de tao gia tri | Neu context nam trong email/call/Slack qua nhieu, tool thieu du lieu | Alternatives hien tai dung Jira/Confluence | Test import du lieu that tu 2-3 du an |
| A5: Khach hang chap nhan cach lam AI-assisted | Neu hop dong/bao mat cam dua tai lieu vao AI, bi chan | Enterprise co lo ngai data | Validate voi chinh sach bao mat va option private deployment |

**Assumption nguy hiem nhat neu toi dang sai:**  
> Pain Prepare/Confirm khong du lon hoac khong xay ra thuong xuyen; neu sai, product chi la tool tao ticket dep chu khong giam duoc rework that.

## Buoc 11 - Share trong ban

| Y phan bien toi nghe duoc | No cham vao phan nao? | Toi se giu / sua gi? |
|---|---|---|
| "Dung goi user la cong ty outsource, phai chon PM/Tech Lead hoac BA." | Job executor | Giu PM/Tech Lead lam executor, BA la collaborator |
| "AI tao ticket thi de copy; moat nam o context du an va approval flow." | AI leverage point | Sua hypothesis de nhan manh tich hop Jira/Confluence va human approval |
| "Neu requirement sai tu dau, AI co the lam sai nhanh hon." | Risk / assumptions | Them assumption ve trust, audit trail va validate bang prototype |

## Buoc 12 - Chot version cuoi sau thao luan

### Sau khi nghe phan bien, toi thay doi gi?

- [x] Giu nguyen `job executor`
- [ ] Sua `job executor`
- [ ] Giu nguyen `core JTBD`
- [x] Sua `core JTBD`
- [x] Giu nguyen `AI leverage point`
- [ ] Sua `AI leverage point`
- [ ] Giu nguyen `product hypothesis`
- [x] Sua `product hypothesis`

### Vi sao toi giu / sua?

> Toi giu PM/Tech Lead vi day la nguoi chiu trach nhiem delivery va ra quyet dinh trong sprint planning.  
> Toi sua JTBD va hypothesis de bo bot tu "AI" khoi job statement, dong thoi nhan manh context du an, approval flow va risk log thay vi chi tao ticket tu dong.

### Version cuoi cung toi nop

**Job executor:**  
> Project Manager / Tech Lead trong team outsource phan mem.

**Core JTBD:**  
> Chuyen yeu cau khach hang thanh ke hoach delivery ro rang, co the giao viec va kiem soat duoc truoc khi sprint bat dau.

**2 buoc dau nhat trong workflow:**  
> Prepare va Confirm.

**AI leverage point chinh:**  
> Doc requirement va context du an de tao backlog draft, acceptance criteria, cau hoi clarify va risk log co human approval.

**Product hypothesis:**  
> Neu chung ta giup PM/Tech Lead lam ro requirement va tao backlog co the giao viec o buoc Prepare/Confirm bang AI co context du an va approval flow, ho se chuyen tu Jira + hop thu cong + ChatGPT rieng le sang AI Delivery Copilot vi no giam thoi gian planning va giam rework trong sprint.

**Assumption can validate dau tien:**  
> Prepare/Confirm co phai pain du lon, xay ra du thuong xuyen va dang lam team mat tien/thoi gian vi rework hay khong.

## Checklist truoc khi nop

- [x] Toi da khoanh dung 1 lat cat cu the cua du an.
- [x] Toi da phan biet duoc `job executor` voi buyer / influencer.
- [x] `Core JTBD` cua toi khong nhet solution vao cau.
- [x] Toi da viet du 3 `job stories`.
- [x] Toi da dien `JTBD lite map` va khoanh ra 2 buoc dau nhat.
- [x] Toi da chi ra `AI leverage point` thay vi nhay thang vao feature list.
- [x] Toi da ghi ro `assumptions to validate`.
- [x] Toi da sua version cuoi sau khi share trong ban.


<div align="center">

# 🚀 QA Assistant System & Smart AI-Powered Bug Triage
### نظام مساعد اختبار الجودة المدعوم بالذكاء الاصطناعي لفرز وإدارة الباجات بذكاء وفعالية[cite: 1, 2]

[![Team](https://img.shields.io/badge/Team-Bug%20Busters1-orange.svg)](https://github.com/Bug-Busters1)
[![Academic Year](https://img.shields.io/badge/Academic%20Year-2026%E2%80%932027-blue.svg)](https://github.com/Bug-Busters1)
[![Status](https://img.shields.io/badge/Status-In%20Development-yellow.svg)](https://github.com/Bug-Busters1/qa-ai-bug-triage)
[![AI Powered](https://img.shields.io/badge/AI-Powered%20Triage-success.svg)](https://github.com/Bug-Busters1/qa-ai-bug-triage)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Bug-Busters1/qa-ai-bug-triage)

*نظام ذكي متكامل لدعم فرق اختبار البرمجيات، تحسين تقارير العيوب، وتسريع عملية الفرز والتصنيف باستخدام أحدث تقنيات الذكاء الاصطناعي[cite: 1, 2].*

[المقدمة](#-1-مقدمة-النطاق الوظيفي) • [الأدوار](#-2-أدوار-المستخدمين-والأذونات) • [المتطلبات](#-3-تفاصيل-متطلبات-الوظائف-functional-requirements---frs) • [التقنيات](#-4-التقنيات-المقترحة-tech-stack) • [خريطة الطريق](#-5-خريطة-الطريق-roadmap) • [الهيكل](#-6-هيكل-المشروع)

</div>

---

## 📌 1. مقدمة النطاق الوظيفي (Project Overview)
يُعد نظام **QA Assistant System & Smart AI-Powered Bug Triage** منصة ويب ذكية صُممت خصيصاً لمساعدة فرق الـ QA والمطورين في تجاوز عقبات إدارة الباجات التقليدية[cite: 1, 2]. من خلال دمج قدرات الذكاء الاصطناعي (AI/NLP)، يساعد النظام في اقتراح درجات الخطورة والأولوية، اكتشاف الباجات المكررة، تلخيص العيوب، واقتراح المطور المسؤول، مع إبقاء القرار النهائي بيد العنصر البشري[cite: 2, 4].

* **فريق العمل:** Bug Busters1[cite: 1]
* **المشرف الأكاديمي:** Ahmed Abd Elhafez[cite: 1]
* **مهندس الجودة (QA Engineer):** Abd Elrahman Esmat[cite: 1]
* **السنة الدراسية:** 2026–2027[cite: 1]

---

## 👥 2. أدوار المستخدمين والأذونات (Target Users & Roles)
يحدد النظام صلاحيات دقيقة بناءً على أدوار المستخدمين (RBAC):

| الدور (Role) | الصلاحيات والمسؤوليات الرئيسية |
| :--- | :--- |
| **QA Engineers & Testers** | تسجيل الباجات، كتابة وتنفيذ حالات الاختبار، مراجعة مقترحات الـ AI، وتتبع الحلول. |
| **QA Team Leaders** | مراجعة وترتيب أولويات العيوب، مراقبة أنشطة التفتيش والاختبار للفريق، وتعيين المهام وتحليل الأداء. |
| **Software Developers** | استعراض الباجات المسندة إليهم، مراجعة خطوات إعادة إنتاج الخطأ، تحديث حالات الأخطاء وتسجيل الحل. |
| **Project Managers** | مراقبة تقدم المشروع، مراجعة إحصائيات وعيوب السيستم، تحديد اختناقات الاختبار وتقييم الجودة. |

---

## 📋 3. تفاصيل متطلبات الوظائف (Functional Requirements - FRs)

### أ) وحدة إدارة المستخدمين والمصادقة (User Management & Authentication)
* **FR-AUTH-01:** توفير واجهة آمنة لتسجيل الحسابات وتسجيل الدخول.
* **FR-AUTH-02:** تطبيق صلاحيات الوصول (RBAC) بناءً على دور المستخدم.
* **FR-AUTH-03:** إدارة وتحديث الملف الشخصي للمستخدم.

### ب) وحدة الإبلاغ عن الأخطاء وإدارتها (Bug Management)
* **FR-BUG-01:** إنشاء تقرير خطأ شامل (العنوان، الوصف، خطوات التكرار، النتيجة المتوقعة والفعلية، وبيئة التشغيل).
* **FR-BUG-02:** تتبع وتحديث حالة العيوب (`Open`، `Resolved`، `Closed`).
* **FR-BUG-03:** توفير أدوات بحث متقدمة وفلاتر للوصول السريع للباجات.

### ج) وحدة الفرز الذكي المدعومة بالذكاء الاصطناعي (AI-Powered Bug Triage)
* **FR-AI-01:** قراءة وتحليل وصف تقرير الخطأ آلياً بواسطة الـ AI.
* **FR-AI-02:** اقتراح مستويات الخطورة (`Severity`) والأولوية (`Priority`).
* **FR-AI-03:** تصنيف الأخطاء تلقائياً إلى فئاتها المحددة.
* **FR-AI-04:** فحص قاعدة البيانات لكشف الباجات المكررة (`Potential Duplicates`).
* **FR-AI-05:** توليد ملخصات سريعة ومركزة للعيوب المبلغ عنها.
* **FR-AI-06:** اقتراح المطور أو الفريق الأنسب لإسناد الباغ إليه.

### د) وحدة إدارة حالات الاختبار (Test Case Management)
* **FR-TC-01:** إنشاء وتعديل حالات الاختبار (`Test Cases`)[cite: 4].
* **FR-TC-02:** تسجيل نتائج التنفيذ (`Pass` / `Fail` / `Blocked`)[cite: 4].
* **FR-TC-03:** ربط حالات الاختبار بتقارير الأخطاء ذات الصلة[cite: 4].

### هـ) لوحة التحكم والتقارير (Dashboard & Reporting)
* **FR-DASH-01:** عرض الإحصائيات العامة لإجمالي الباجات في منصة مركزية[cite: 4].
* **FR-DASH-02:** عرض العدادات الحية للباجات (المفتوحة، قيد الحل، والمغلقة)[cite: 4].
* **FR-DASH-03:** تقديم رسوم بيانية تفاعلية لتوزيع الأخطاء حسب الشدة والنوع[cite: 4].
* **FR-DASH-04:** متابعة مؤشرات أداء الجودة (`KPIs`)[cite: 4].

### و) المراجعة البشرية والتغذية الراجعة (Human Review & Feedback)
* **FR-REV-01:** السماح للمستخدم بقبول أو تعديل مقترحات الذكاء الاصطناعي[cite: 4].
* **FR-REV-02:** حفظ وتسجيل التقييم والتصنيف النهائي المعتمد بشرياً[cite: 4].
* **FR-REV-03:** جمع الـ Feedback لتقييم تحسين دقة الـ AI مستقبلاً[cite: 4].

---

## 🛠️ 4. التقنيات المقترحة (Tech Stack)
* **Frontend:** React / Next.js, TypeScript, Tailwind CSS
* **Backend:** Python (FastAPI) أو Node.js (NestJS / Express)
* **Database:** PostgreSQL + Redis (للتخزين المؤقت وتحسين الأداء)
* **AI Layer:** OpenAI / Gemini API / Local LLMs + Vector Embeddings للكشف عن المكررات
* **Auth & Security:** JWT + Role-Based Access Control (RBAC)
* **Charts & Analytics:** Recharts / Chart.js
* **Version Control & Deployment:** Git, GitHub, Docker, Vercel / Railway

---

## 🚀 5. خريطة الطريق (Roadmap)
- [x] تحليل المتطلبات الوظيفية وتوثيقها (`FRD`)
- [ ] تصميم هيكل قاعدة البيانات وواجهات المستخدم (`UI/UX`)
- [ ] تطوير وحدة المصادقة وإدارة الصلاحيات (`Auth Module`)
- [ ] بناء وحدة الإبلاغ عن الأخطاء (`Bug Management`)
- [ ] دمج طبقة الذكاء الاصطناعي (`AI Triage & Duplicate Detection`)
- [ ] تطوير وحدة حالات الاختبار (`Test Cases`)
- [ ] بناء لوحة التحكم والرسوم البيانية (`Dashboard & Charts`)
- [ ] تفعيل نظام المراجعة البشرية والتغذية الراجعة
- [ ] إجراء الاختبارات الشاملة والتوثيق النهائي (`Testing & QA`)
- [ ] النشر والاطلاق الرسمي (`Deployment`)

---

## 📁 6. هيكل المشروع المقترح (Repository Structure)
```text
qa-ai-bug-triage/
├── frontend/             # واجهة المستخدم (Client-side UI)
├── backend/              # خادم الـ API والخدمات الأساسية
├── ai-service/           # خدمة الذكاء الاصطناعي ومعالجة النصوص
├── docs/                 # التوثيق ومستندات المتطلبات (FRD / NFRD)
├── docker-compose.yml    # إعداد الحاويات والبنية التحتية
└── README.md             # توثيق المشروع الرئيسي

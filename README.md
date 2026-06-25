# Light Superpowers

Light Superpowers is a lightweight Codex workflow plugin for people who like the discipline of Superpowers but do not want full brainstorming, planning, TDD, subagent, worktree, or branch-completion ceremony for every small task.

## Languages

- [English](#english)
- [简体中文](#简体中文)
- [繁體中文](#繁體中文)
- [日本語](#日本語)
- [한국어](#한국어)
- [Español](#español)
- [Français](#français)
- [Deutsch](#deutsch)
- [Italiano](#italiano)
- [Português](#português)
- [Русский](#русский)
- [العربية](#العربية)
- [हिन्दी](#हिन्दी)
- [Bahasa Indonesia](#bahasa-indonesia)

## Install

Add this repository as a Codex plugin marketplace:

```powershell
codex plugin marketplace add eqa1231/light-superpowers --ref main
```

Then install the plugin:

```powershell
codex plugin add light-superpowers@light-superpowers
```

Open a new Codex thread after installation so the skill index refreshes.

## Use

Invoke the skill explicitly when you want a task-sized workflow:

```text
Use $light-superpowers and keep this task lightweight.
```

Useful prompts:

```text
Use $light-superpowers: make the smallest safe change and verify it.
```

```text
Use $light-superpowers instead of the full Superpowers workflow.
```

## Repository Layout

```text
.agents/plugins/marketplace.json
plugins/light-superpowers/.codex-plugin/plugin.json
plugins/light-superpowers/skills/light-superpowers/SKILL.md
```

## English

### What Problem Does It Solve?

Full Superpowers-style workflows are valuable for large, risky engineering tasks, but they can feel too heavy for small edits, quick checks, documentation updates, or clearly scoped bug fixes. Light Superpowers solves that mismatch by scaling the workflow to the task.

### What It Does

- Keeps small tasks small.
- Uses short plans only when the work needs them.
- Avoids full brainstorming, design documents, subagents, worktrees, and branch workflows unless the task is high risk or the user asks.
- Keeps verification, but scales it to the task.
- Leaves project-specific rules and repository guidance in charge.

## 简体中文

### 解决了什么问题？

完整的 Superpowers 工作流很适合大型、高风险研发任务，但对小改动、快速查询、文档更新、边界清晰的 bugfix 来说，经常显得过重。Light Superpowers 解决的是“流程强度和任务大小不匹配”的问题。

### 它做什么？

- 让小任务保持轻量，不强行进入完整仪式。
- 只有任务需要时才输出简短计划。
- 默认不启用完整 brainstorming、设计文档、子 Agent、worktree、分支收尾流程。
- 保留必要验证，但验证范围跟随任务风险缩放。
- 不覆盖项目自己的 AGENTS、规范、架构规则和仓库约定。

## 繁體中文

### 解決了什麼問題？

完整的 Superpowers 工作流很適合大型、高風險的工程任務，但對小修改、快速檢查、文件更新、範圍清楚的 bugfix 來說，常常顯得太重。Light Superpowers 解決的是「流程強度和任務大小不匹配」的問題。

### 它做什麼？

- 讓小任務保持輕量，不強行進入完整儀式。
- 只有任務需要時才使用簡短計畫。
- 預設不啟用完整 brainstorming、設計文件、子 Agent、worktree、分支收尾流程。
- 保留必要驗證，但驗證範圍會隨任務風險縮放。
- 不覆蓋專案自己的 AGENTS、規範、架構規則和倉庫約定。

## 日本語

### 何を解決しますか？

完全な Superpowers 形式のワークフローは、大きくてリスクの高い開発には役立ちます。しかし、小さな修正、簡単な確認、ドキュメント更新、範囲が明確なバグ修正には重すぎることがあります。Light Superpowers は、タスクの大きさに合わせてワークフローを軽くするためのプラグインです。

### 何をしますか？

- 小さなタスクを小さなまま進めます。
- 必要な場合だけ短い計画を使います。
- 高リスクな作業やユーザーの明示的な依頼がない限り、完全な brainstorming、設計文書、subagent、worktree、ブランチ完了フローを使いません。
- 検証は残しつつ、タスクのリスクに合わせて範囲を調整します。
- プロジェクト固有のルールやリポジトリのガイドラインを優先します。

## 한국어

### 어떤 문제를 해결하나요?

전체 Superpowers 방식의 워크플로는 크고 위험도가 높은 개발 작업에는 유용하지만, 작은 수정, 빠른 확인, 문서 업데이트, 범위가 명확한 버그 수정에는 과하게 느껴질 수 있습니다. Light Superpowers는 작업 크기에 맞게 워크플로의 무게를 조절합니다.

### 무엇을 하나요?

- 작은 작업은 작게 유지합니다.
- 필요한 경우에만 짧은 계획을 사용합니다.
- 고위험 작업이거나 사용자가 요청하지 않는 한 전체 brainstorming, 설계 문서, subagent, worktree, 브랜치 마무리 흐름을 사용하지 않습니다.
- 검증은 유지하되 작업 위험도에 맞게 범위를 조절합니다.
- 프로젝트별 규칙과 저장소 가이드를 우선합니다.

## Español

### ¿Qué Problema Resuelve?

Los flujos completos al estilo Superpowers son útiles para tareas grandes o riesgosas, pero pueden ser demasiado pesados para cambios pequeños, revisiones rápidas, documentación o correcciones de bugs bien acotadas. Light Superpowers ajusta el flujo de trabajo al tamaño real de la tarea.

### ¿Qué Hace?

- Mantiene pequeñas las tareas pequeñas.
- Usa planes cortos solo cuando el trabajo lo necesita.
- Evita brainstorming completo, documentos de diseño, subagentes, worktrees y flujos de cierre de ramas salvo que haya alto riesgo o el usuario lo pida.
- Conserva la verificación, pero la ajusta al riesgo de la tarea.
- Respeta las reglas del proyecto y las guías del repositorio.

## Français

### Quel Problème Résout-Il ?

Les workflows complets de type Superpowers sont utiles pour les tâches importantes ou risquées, mais ils peuvent être trop lourds pour de petites modifications, des vérifications rapides, de la documentation ou des corrections de bug bien délimitées. Light Superpowers adapte le workflow à la taille réelle de la tâche.

### Que Fait-Il ?

- Garde les petites tâches légères.
- Utilise des plans courts uniquement quand le travail l'exige.
- Évite le brainstorming complet, les documents de conception, les sous-agents, les worktrees et les workflows de fin de branche sauf en cas de risque élevé ou de demande explicite.
- Conserve la vérification, mais l'adapte au risque de la tâche.
- Respecte les règles du projet et les conventions du dépôt.

## Deutsch

### Welches Problem Löst Es?

Vollständige Superpowers-Workflows sind bei großen oder riskanten Entwicklungsaufgaben hilfreich, wirken aber bei kleinen Änderungen, schnellen Prüfungen, Dokumentationsarbeiten oder klar eingegrenzten Bugfixes oft zu schwer. Light Superpowers passt den Workflow an die tatsächliche Größe der Aufgabe an.

### Was Macht Es?

- Kleine Aufgaben bleiben klein.
- Kurze Pläne werden nur genutzt, wenn die Arbeit sie braucht.
- Vollständiges Brainstorming, Designdokumente, Subagents, Worktrees und Branch-Abschlussflows werden nur bei hohem Risiko oder auf Wunsch genutzt.
- Verifikation bleibt erhalten, wird aber an das Aufgabenrisiko angepasst.
- Projektregeln und Repository-Konventionen haben Vorrang.

## Italiano

### Quale Problema Risolve?

I workflow completi in stile Superpowers sono utili per attività grandi o rischiose, ma possono essere troppo pesanti per piccole modifiche, controlli rapidi, aggiornamenti della documentazione o bugfix ben delimitati. Light Superpowers adatta il flusso di lavoro alla dimensione reale del compito.

### Cosa Fa?

- Mantiene leggere le attività piccole.
- Usa piani brevi solo quando servono davvero.
- Evita brainstorming completo, documenti di design, subagent, worktree e flussi di chiusura dei branch salvo rischio elevato o richiesta esplicita.
- Mantiene la verifica, ma ne adatta l'ambito al rischio del compito.
- Rispetta le regole del progetto e le convenzioni del repository.

## Português

### Que Problema Ele Resolve?

Fluxos completos no estilo Superpowers são úteis para tarefas grandes ou arriscadas, mas podem ser pesados demais para pequenas mudanças, verificações rápidas, documentação ou correções de bugs bem delimitadas. Light Superpowers ajusta o fluxo de trabalho ao tamanho real da tarefa.

### O Que Ele Faz?

- Mantém pequenas as tarefas pequenas.
- Usa planos curtos apenas quando o trabalho precisa.
- Evita brainstorming completo, documentos de design, subagentes, worktrees e fluxos de finalização de branch, exceto quando houver alto risco ou pedido explícito.
- Mantém a verificação, mas ajusta seu escopo ao risco da tarefa.
- Respeita as regras do projeto e as orientações do repositório.

## Русский

### Какую Проблему Он Решает?

Полные рабочие процессы в стиле Superpowers полезны для крупных и рискованных инженерных задач, но могут быть слишком тяжелыми для небольших правок, быстрых проверок, обновления документации или четко ограниченных исправлений. Light Superpowers подстраивает процесс под реальный размер задачи.

### Что Он Делает?

- Не утяжеляет маленькие задачи.
- Использует короткие планы только тогда, когда они действительно нужны.
- Не включает полное brainstorming, дизайн-документы, subagents, worktrees и финальные branch-процессы без высокого риска или явного запроса пользователя.
- Сохраняет проверку, но масштабирует ее под риск задачи.
- Уважает правила проекта и соглашения репозитория.

## العربية

### ما المشكلة التي يحلها؟

تكون تدفقات العمل الكاملة بأسلوب Superpowers مفيدة للمهام الهندسية الكبيرة أو عالية المخاطر، لكنها قد تكون ثقيلة جدا على التعديلات الصغيرة، والفحوصات السريعة، وتحديثات التوثيق، وإصلاحات الأخطاء محددة النطاق. يحل Light Superpowers هذه المشكلة بجعل حجم سير العمل مناسبا لحجم المهمة.

### ماذا يفعل؟

- يبقي المهام الصغيرة خفيفة.
- يستخدم خطة قصيرة فقط عندما تحتاج المهمة إلى ذلك.
- يتجنب brainstorming الكامل، ووثائق التصميم، وsubagents، وworktrees، وتدفقات إنهاء الفروع إلا عند وجود مخاطرة عالية أو طلب صريح من المستخدم.
- يحافظ على التحقق، لكنه يضبط نطاقه حسب مخاطر المهمة.
- يعطي الأولوية لقواعد المشروع وإرشادات المستودع.

## हिन्दी

### यह कौन सी समस्या हल करता है?

पूरे Superpowers जैसे workflow बड़े और जोखिम भरे engineering tasks के लिए उपयोगी होते हैं, लेकिन छोटे edits, quick checks, documentation updates, या clearly scoped bug fixes के लिए वे अक्सर बहुत भारी लगते हैं। Light Superpowers workflow को task के वास्तविक आकार के अनुसार हल्का करता है।

### यह क्या करता है?

- छोटे tasks को हल्का और सीधा रखता है।
- केवल जरूरत होने पर छोटा plan इस्तेमाल करता है।
- High-risk task या user request के बिना full brainstorming, design documents, subagents, worktrees, और branch completion flows नहीं चलाता।
- Verification बनाए रखता है, लेकिन उसका scope task risk के अनुसार तय करता है।
- Project rules और repository guidance को प्राथमिकता देता है।

## Bahasa Indonesia

### Masalah Apa yang Diselesaikan?

Workflow lengkap bergaya Superpowers berguna untuk pekerjaan engineering yang besar atau berisiko tinggi, tetapi bisa terasa terlalu berat untuk perubahan kecil, pengecekan cepat, pembaruan dokumentasi, atau bugfix dengan cakupan jelas. Light Superpowers menyesuaikan workflow dengan ukuran tugas yang sebenarnya.

### Apa yang Dilakukan?

- Menjaga tugas kecil tetap ringan.
- Menggunakan rencana singkat hanya saat diperlukan.
- Menghindari brainstorming penuh, dokumen desain, subagent, worktree, dan alur penyelesaian branch kecuali tugas berisiko tinggi atau diminta pengguna.
- Tetap melakukan verifikasi, tetapi menyesuaikan cakupannya dengan risiko tugas.
- Mengutamakan aturan proyek dan panduan repository.

# AI Context — Sutta Nipata

## What this project is

A static mini site for studying the Sutta Nipata (经集), one of the oldest texts in the Pali Canon. Spoke 8 under The Dharma Gate portal. Same architecture as all other DharmaGate spokes — HTML + external CSS, no frameworks.

## Current state (as of 2026-06-13)

- Phase 3 complete — ready for Phase 4 (deploy)
- All 71 section pages written and complete
- index.html: complete (vagga-grouped, 71 sutta cards; labels use Chinese 第N品·第M经 format)
- Card labels on index and section h1/nav all aligned to Chinese vagga-relative numbering
- Two bugs fixed: section55.html redundant 序偈 in h1; section46.html duplicate/bad Google Fonts link
- Audit complete: docs/audit-config.json + docs/reference.py created; structure check passes all 71 pages
- Remaining Phase 3 items: manual browser review (toggle, TTS, mobile layout)

## Card pattern (verse-by-verse)

```html
<div class="explanation-card">
  <p class="line"><strong>Primary Chinese text</strong></p>
  <p class="explanation-zh">Chinese explanation (always visible)</p>
  <button class="toggle-btn" onclick="toggleDetail(this)" aria-expanded="false">English ▾</button>
  <div class="detail-content" hidden>
    <p class="translation">Bhikkhu Bodhi English translation (red)</p>
    <p class="explanation">English commentary (grey)</p>
  </div>
</div>
```

## Summary pattern

```html
<section class="summary">
  <h2>总结 · Summary</h2>
  <p class="summary-zh">Chinese summary</p>
  <button class="toggle-btn" onclick="toggleDetail(this)" aria-expanded="false">English ▾</button>
  <div class="detail-content" hidden>
    <p class="explanation">English summary</p>
  </div>
</section>
```

## Content sources

- **Chinese primary text (Vagga 4, sections 39–54)**: T0198 义足经 — Zhi Qian, 3rd century
- **Chinese primary text (Vaggas 1–3, 5)**: Modern Chinese translation
- **English translation**: Bhikkhu Bodhi (Wisdom Publications, 2017)
- **Chinese explanations**: Written for this site — accessible modern Chinese
- **English commentary**: Written for this site — contextual, practical

## Sutta map

| Section | Vagga | Sutta | Chinese name |
|---------|-------|-------|--------------|
| section1 | 1 | Uraga | 蛇经 |
| section2 | 1 | Dhaniya | 陀尼耶经 |
| section3 | 1 | Khaggavisāṇa | 犀角经 |
| section4 | 1 | Kasibhāradvāja | 耕田婆罗堕阇经 |
| section5 | 1 | Cunda | 纯陀经 |
| section6 | 1 | Parābhava | 败亡经 |
| section7 | 1 | Vasala | 贱民经 |
| section8 | 1 | Metta | 慈经 |
| section9 | 1 | Hemavata | 雪山夜叉经 |
| section10 | 1 | Āḷavaka | 阿罗婆经 |
| section11 | 1 | Vijaya | 胜利经 |
| section12 | 1 | Muni | 牟尼经 |
| section13 | 2 | Ratana | 宝经 |
| section14 | 2 | Āmagandha | 腥臭经 |
| section15 | 2 | Hirī | 羞耻经 |
| section16 | 2 | Maṅgala | 吉祥经 |
| section17 | 2 | Sūciloma | 针毛经 |
| section18 | 2 | Sammāparibbājanīya | 正游行经 |
| section19 | 2 | Brahmadhammika | 梵法经 |
| section20 | 2 | Nāvā | 船经 |
| section21 | 2 | Kiṃsīla | 何戒经 |
| section22 | 2 | Uṭṭhāna | 起立经 |
| section23 | 2 | Rāhula | 罗睺罗经 |
| section24 | 2 | Vaṅgīsa | 万祇沙经 |
| section25 | 2 | Sammā | 正经 |
| section26 | 2 | Dhammika | 法经 |
| section27 | 3 | Pabbajjā | 出家经 |
| section28 | 3 | Padhāna | 精进经 |
| section29 | 3 | Subhāsita | 善说经 |
| section30 | 3 | Sundarikabhāradvāja | 孙陀利经 |
| section31 | 3 | Māgha | 摩伽经 |
| section32 | 3 | Sabhiya | 沙毗耶经 |
| section33 | 3 | Sela | 沙罗经 |
| section34 | 3 | Salla | 箭经 |
| section35 | 3 | Vāseṭṭha | 婆私吒经 |
| section36 | 3 | Kokāliya | 瞿迦梨经 |
| section37 | 3 | Nālaka | 那罗迦经 |
| section38 | 3 | Dvayatānupassanā | 二随观经 |
| section39 | 4 (T0198) | Kāma | 欲经 |
| section40 | 4 (T0198) | Guhaṭṭhaka | 洞穴八偈 |
| section41 | 4 (T0198) | Duṭṭhaṭṭhaka | 恶意八偈 |
| section42 | 4 (T0198) | Suddhaṭṭhaka | 清净八偈 |
| section43 | 4 (T0198) | Paramaṭṭhaka | 最上八偈 |
| section44 | 4 (T0198) | Jarā | 老经 |
| section45 | 4 (T0198) | Tissametteyya | 帝须弥勒经 |
| section46 | 4 (T0198) | Pasūra | 波须罗经 |
| section47 | 4 (T0198) | Māgandiya | 摩犍提经 |
| section48 | 4 (T0198) | Purābheda | 死前经 |
| section49 | 4 (T0198) | Kalahavivāda | 诤论经 |
| section50 | 4 (T0198) | Cūḷaviyūha | 小阵列经 |
| section51 | 4 (T0198) | Mahāviyūha | 大阵列经 |
| section52 | 4 (T0198) | Tuvaṭaka | 迅速经 |
| section53 | 4 (T0198) | Attadaṇḍa | 执杖经 |
| section54 | 4 (T0198) | Sāriputta | 舍利弗经 |
| section55 | 5 | Vatthugāthā | 序偈 |
| section56 | 5 | Ajita | 阿耆多经 |
| section57 | 5 | Tissametteyya | 帝须弥勒经 |
| section58 | 5 | Puṇṇaka | 富楼那经 |
| section59 | 5 | Mettagū | 弥多求经 |
| section60 | 5 | Dhotaka | 道多迦经 |
| section61 | 5 | Upasīva | 优婆私婆经 |
| section62 | 5 | Nanda | 难陀经 |
| section63 | 5 | Hemaka | 醯摩迦经 |
| section64 | 5 | Todeyyaputta | 都提耶经 |
| section65 | 5 | Kappa | 迦波经 |
| section66 | 5 | Jatukaṇṇī | 闍兔甘尼经 |
| section67 | 5 | Bhadrāvudha | 跋陀卫经 |
| section68 | 5 | Udaya | 优陀耶经 |
| section69 | 5 | Posāla | 褒沙罗经 |
| section70 | 5 | Mogharājā | 谟伽罗阇经 |
| section71 | 5 | Piṅgiya | 宾耆耶经 |

## Section page nav pattern

- section1.html: `目录 Contents` only (no prev)
- section71.html: `← 第五品·第十五经` · `目录 Contents` only (no next)
- All others: `← 第N品·第M经` · `目录 Contents` · `第N品·第M经 →`
- Nav labels use Chinese vagga-relative numbering (e.g. `第五品·第三经`), not sequential

## Speech button

🔊 聆听经文 — targets Ting-Ting voice on iOS Safari (zh-CN, rate 0.9)

## Portal link

Portal bar and footer both link to: `https://lugh3456.github.io/DharmaGate/`

## GitHub repo

Live URL (when deployed): `https://lugh3456.github.io/SuttaNipata/`
Repository: `https://github.com/Lugh3456/SuttaNipata`

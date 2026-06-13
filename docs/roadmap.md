# Roadmap — Sutta Nipata

## Phase 1 — Project setup

- [x] Research: content decisions (translation, Chinese layer, format)
- [x] Create folder structure (css/, docs/, Backup/)
- [x] Copy style.css from Dhammapada
- [x] Create docs: ai-context.md, architecture.md, plan.md, roadmap.md, readme.md
- [x] Build index.html (vagga-grouped, 71 sutta cards)

## Phase 2 — Section pages

### Vagga 1 — 蛇品 Uragavagga
- [x] section1.html — Uraga 蛇经
- [x] section2.html — Dhaniya 陀尼耶经
- [x] section3.html — Khaggavisāṇa 犀角经
- [x] section4.html — Kasibhāradvāja 耕田婆罗堕阇经
- [x] section5.html — Cunda 纯陀经
- [x] section6.html — Parābhava 败亡经
- [x] section7.html — Vasala 贱民经
- [x] section8.html — Metta 慈经
- [x] section9.html — Hemavata 雪山夜叉经
- [x] section10.html — Āḷavaka 阿罗婆经
- [x] section11.html — Vijaya 胜利经
- [x] section12.html — Muni 牟尼经

### Vagga 2 — 小品 Cūḷavagga
- [x] section13.html — Ratana 宝经
- [x] section14.html — Āmagandha 腥臭经
- [x] section15.html — Hirī 羞耻经
- [x] section16.html — Maṅgala 吉祥经
- [x] section17.html — Sūciloma 针毛经
- [x] section18.html — Sammāparibbājanīya 正游行经
- [x] section19.html — Brahmadhammika 梵法经
- [x] section20.html — Nāvā 船经
- [x] section21.html — Kiṃsīla 何戒经
- [x] section22.html — Uṭṭhāna 起立经
- [x] section23.html — Rāhula 罗睺罗经
- [x] section24.html — Vaṅgīsa 万祇沙经
- [x] section25.html — Sammā 正经
- [x] section26.html — Dhammika 法经

### Vagga 3 — 大品 Mahāvagga
- [x] section27.html — Pabbajjā 出家经
- [x] section28.html — Padhāna 精进经
- [x] section29.html — Subhāsita 善说经
- [x] section30.html — Sundarikabhāradvāja 孙陀利经
- [x] section31.html — Māgha 摩伽经
- [x] section32.html — Sabhiya 沙毗耶经
- [x] section33.html — Sela 沙罗经
- [x] section34.html — Salla 箭经
- [x] section35.html — Vāseṭṭha 婆私吒经
- [x] section36.html — Kokāliya 瞿迦梨经
- [x] section37.html — Nālaka 那罗迦经
- [x] section38.html — Dvayatānupassanā 二随观经

### Vagga 4 — 八偈品 Aṭṭhakavagga (T0198 义足经)
- [x] section39.html — Kāma 欲经
- [x] section40.html — Guhaṭṭhaka 洞穴八偈
- [x] section41.html — Duṭṭhaṭṭhaka 恶意八偈
- [x] section42.html — Suddhaṭṭhaka 清净八偈
- [x] section43.html — Paramaṭṭhaka 最上八偈
- [x] section44.html — Jarā 老经
- [x] section45.html — Tissametteyya 帝须弥勒经
- [x] section46.html — Pasūra 波须罗经
- [x] section47.html — Māgandiya 摩犍提经
- [x] section48.html — Purābheda 死前经
- [x] section49.html — Kalahavivāda 诤论经
- [x] section50.html — Cūḷaviyūha 小阵列经
- [x] section51.html — Mahāviyūha 大阵列经
- [x] section52.html — Tuvaṭaka 迅速经
- [x] section53.html — Attadaṇḍa 执杖经
- [x] section54.html — Sāriputta 舍利弗经

### Vagga 5 — 彼岸道品 Pārāyanavagga
- [x] section55.html — Vatthugāthā 序偈
- [x] section56.html — Ajita 阿耆多经
- [x] section57.html — Tissametteyya 帝须弥勒经
- [x] section58.html — Puṇṇaka 富楼那经
- [x] section59.html — Mettagū 弥多求经
- [x] section60.html — Dhotaka 道多迦经
- [x] section61.html — Upasīva 优婆私婆经
- [x] section62.html — Nanda 难陀经
- [x] section63.html — Hemaka 醯摩迦经
- [x] section64.html — Todeyya 都提耶经
- [x] section65.html — Kappa 迦波经
- [x] section66.html — Jatukaṇṇī 闍兔甘尼经
- [x] section67.html — Bhadrāvudha 跋陀卫经
- [x] section68.html — Udaya 优陀耶经
- [x] section69.html — Posāla 褒沙罗经
- [x] section70.html — Mogharājā 谟伽罗阇经
- [x] section71.html — Piṅgiya 宾耆耶经

## Phase 3 — Local review & audit

- [ ] Review all 71 section pages locally in browser
- [ ] Check toggle functionality on all pages
- [ ] Check TTS (🔊 button) on iOS Safari
- [ ] Check responsive layout on mobile
- [ ] Verify all prev/next nav links are correct
- [x] Run audit script (reference.py + audit-config.json) — structure check: all 71 pages clean; content audit false positives due to verse/dialogue format (expected)

## Phase 4 — Deploy

- [ ] Create GitHub repository: `SuttaNipata`
- [ ] Push all files to main branch
- [ ] Verify live on GitHub Pages: https://lugh3456.github.io/SuttaNipata/
- [ ] Activate card in DharmaGate portal (remove COMING SOON badge, add link)
- [ ] Update DharmaGate docs (ai-context.md, roadmap.md)
- [ ] Deploy updated DharmaGate to GitHub Pages

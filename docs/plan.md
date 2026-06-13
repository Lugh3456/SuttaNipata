# Plan — Sutta Nipata

## Vision

A clean, bilingual study site for the Sutta Nipata (经集) — one of the oldest Buddhist texts in the Pali Canon. Each of the 71 suttas is presented verse by verse, with classical or modern Chinese as the primary layer, accessible Chinese commentary always visible, and Bhikkhu Bodhi's English translation + commentary available on toggle.

The site is spoke 8 in The Dharma Gate portal, following the same architecture and design system as all other DharmaGate scripture sites.

## Objectives

1. Make the Sutta Nipata accessible for personal study — annotated, not raw scripture
2. Maintain the bilingual Chinese-first format consistent with all other DharmaGate sites
3. Include every sutta and verse — no cutting or condensing of the primary text
4. Present Bhikkhu Bodhi's translation faithfully alongside contextual English commentary

## Content Approach

- **Primary text (Vagga 4)**: T0198 义足经 — Zhi Qian's classical Chinese translation of the Aṭṭhakavagga (3rd century)
- **Primary text (Vaggas 1–3, 5)**: Modern Chinese translation (no complete classical Taishō equivalent exists)
- **Chinese explanation**: Modern, accessible Chinese — concept-focused, 2–4 sentences per sutta passage
- **English translation**: Bhikkhu Bodhi (Wisdom Publications, 2017) — reproduced accurately
- **English commentary**: Contextual explanation — practical, grounded
- **Chapter summary**: Chinese (always visible) + English (toggle) — covers the sutta theme and key takeaways

## Scope

- 5 vaggas, 71 suttas total
- One HTML file per sutta (section1.html through section71.html)
- index.html uses a vagga-grouped card layout (5 vagga sections, 71 sutta cards)

### Sutta map

**Vagga 1 — 蛇品 Uragavagga** — section1–12
1. Uraga (蛇经) · 2. Dhaniya (陀尼耶经) · 3. Khaggavisāṇa (犀角经) · 4. Kasibhāradvāja (耕田婆罗堕阇经) · 5. Cunda (纯陀经) · 6. Parābhava (败亡经) · 7. Vasala (贱民经) · 8. Metta (慈经) · 9. Hemavata (雪山夜叉经) · 10. Āḷavaka (阿罗婆经) · 11. Vijaya (胜利经) · 12. Muni (牟尼经)

**Vagga 2 — 小品 Cūḷavagga** — section13–26
13. Ratana (宝经) · 14. Āmagandha (腥臭经) · 15. Hirī (羞耻经) · 16. Maṅgala (吉祥经) · 17. Sūciloma (针毛经) · 18. Sammāparibbājanīya (正游行经) · 19. Brahmadhammika (梵法经) · 20. Nāvā (船经) · 21. Kiṃsīla (何戒经) · 22. Uṭṭhāna (起立经) · 23. Rāhula (罗睺罗经) · 24. Vaṅgīsa (万祇沙经) · 25. Sammā (正经) · 26. Dhammika (法经)

**Vagga 3 — 大品 Mahāvagga** — section27–38
27. Pabbajjā (出家经) · 28. Padhāna (精进经) · 29. Subhāsita (善说经) · 30. Sundarikabhāradvāja (孙陀利经) · 31. Māgha (摩伽经) · 32. Sabhiya (沙毗耶经) · 33. Sela (沙罗经) · 34. Salla (箭经) · 35. Vāseṭṭha (婆私吒经) · 36. Kokāliya (瞿迦梨经) · 37. Nālaka (那罗迦经) · 38. Dvayatānupassanā (二随观经)

**Vagga 4 — 八偈品 Aṭṭhakavagga** — section39–54 *(T0198 义足经)*
39. Kāma (欲经) · 40. Guhaṭṭhaka (洞穴八偈) · 41. Duṭṭhaṭṭhaka (恶意八偈) · 42. Suddhaṭṭhaka (清净八偈) · 43. Paramaṭṭhaka (最上八偈) · 44. Jarā (老经) · 45. Tissametteyya (帝须弥勒经) · 46. Pasūra (波须罗经) · 47. Māgandiya (摩犍提经) · 48. Purābheda (死前经) · 49. Kalahavivāda (诤论经) · 50. Cūḷaviyūha (小阵列经) · 51. Mahāviyūha (大阵列经) · 52. Tuvaṭaka (迅速经) · 53. Attadaṇḍa (执杖经) · 54. Sāriputta (舍利弗经)

**Vagga 5 — 彼岸道品 Pārāyanavagga** — section55–71
55. Vatthugāthā (序偈) · 56. Ajita (阿耆多经) · 57. Tissametteyya (帝须弥勒经) · 58. Puṇṇaka (富楼那经) · 59. Mettagū (弥多求经) · 60. Dhotaka (道多迦经) · 61. Upasīva (优婆私婆经) · 62. Nanda (难陀经) · 63. Hemaka (醯摩迦经) · 64. Todeyyaputta (都提耶经) · 65. Kappa (迦波经) · 66. Jatukaṇṇī (闍兔甘尼经) · 67. Bhadrāvudha (跋陀卫经) · 68. Udaya (优陀耶经) · 69. Posāla (褒沙罗经) · 70. Mogharājā (谟伽罗阇经) · 71. Piṅgiya (宾耆耶经)

## Format

Identical to all other DharmaGate spokes:
- Static HTML + external CSS (no frameworks)
- Same design tokens (red/saffron/cream palette)
- Same card, toggle, and summary patterns
- Same portal bar and footer
- Vagga 4 pages note T0198 as the Chinese source

## Deployment

- Build everything locally first
- Create GitHub repo `SuttaNipata` when all pages are complete
- Push and verify on GitHub Pages
- Activate the card in DharmaGate portal (remove COMING SOON badge)

# Review: `slides/sisj.qmd`

Combined from three Sonnet reviewers (language, accuracy, flow), deduplicated. Items marked ✔ I re-checked myself.
Line numbers refer to the file as of 2026-10-21. You were editing during the review, so expect small drift.
Nothing in the deck has been changed.

---

## 1. Must fix: factual errors

### 1.1 Surgisphere / *The Lancet* (L660, L971) ✔
Current text: "skandal Surgisphere yang mengklaim efektivitas hydroxychloroquine untuk mencegah risiko kematian … yang diamplifikasi Donald Trump … diretraksi *The Lancet* bulan Juli 2020."

- **The claim is reversed.** Mehra et al. (2020) reported that HCQ/CQ was associated with *higher* in-hospital mortality and arrhythmia. That finding briefly led WHO to pause the HCQ arm of its trial.
- **The date is wrong.** The retraction was on **4 June 2020**, not in July.
- **The Trump link describes the wrong thing.** Trump promoted HCQ itself, not this paper; the paper argued against his position. The linked ABC timeline does not mention Surgisphere.
- **The Lancet link points to a different article** ✔. `PIIS0140-6736(20)31528-2` is Funck-Brentano et al., "Retraction and republication: cardiac toxicity of hydroxychloroquine in COVID-19", *Lancet* 396(10245), July 2020. The correct retraction notice is DOI `10.1016/S0140-6736(20)31324-6`.
- **The reference list has the wrong authors** ✔ (L971). The notice is signed by Mehra, **Ruschitzka, Patel** only; Desai did not sign it.
- **Credit is incomplete.** Catherine Offord covered the story extensively. However, the key data investigation was published by *The Guardian* (Davey, Kirchgaessner, Boseley, 3 June 2020).

Suggested replacement:
> Liputan Catherine Offord (*The Scientist*) dan investigasi *The Guardian* mengungkap persoalan data Surgisphere. Artikel di *The Lancet* itu melaporkan bahwa hydroxychloroquine dikaitkan dengan **peningkatan** risiko kematian pasien COVID-19, dan sempat membuat WHO menghentikan sementara uji klinis HCQ. *The Lancet* meretraksinya pada 4 Juni 2020.

### 1.2 Simmons, Nelson & Simonsohn (2011), "When I'm Sixty-Four" (L142)
Current text: "membuat orang **merasa** lebih muda". In Study 2, the participants were *actually* younger: about 1.5 years by birth date, controlling for father's age. That impossible result is the whole point of the paper. "Feeling younger or older" was a different measure, in Study 1, using a different song.

Suggested replacement:
> …"membuktikan" bahwa mendengarkan lagu "*When I'm Sixty-Four*" membuat orang **secara harfiah lebih muda** (hampir 1,5 tahun menurut tanggal lahirnya) — hasil yang mustahil, diperoleh hanya dengan fleksibilitas analisis yang tidak dilaporkan.

### 1.3 Attribution to Charles Piller (L703, L821) ✔
- **The four questions are Pratik Pawar's, not Piller's.** In the Open Notebook piece they appear in Pawar's own voice: "Here are some questions reporters consider…".
- **"Trust, but verify" (L877) is a quote from Richard Van Noorden.** Pawar quotes him saying it in that piece.
- **The "no-surprises email" (L825) is Pawar's own description.** The advice that not responding won't stop publication comes from Van Noorden.

Suggested change for L703: "[Pawar (2022)](…) merangkum empat pertanyaan yang lazim dipakai reporter…". Then at L821, credit only the practices that are actually quoted from each person. At L877, use "(Van Noorden, dalam Pawar, 2022)".

### 1.4 Naudet et al. (2018) (L414)
"17 dari 37 studi **yang dipilih acak**": the 37 were not a random sample. They were *all* eligible RCTs published 2013–2016. The numbers (17/37 and 14/17) are correct.

---

## 2. Broken or incomplete items

| Line | Issue | Fix |
|---|---|---|
| L607 ✔ | The link `#toolkit-yang-bisa-diakses-bebas` points to no slide. | Change it to `#toolkit-yang-bisa-dimanfaatkan`. |
| L215 ✔ | You have filled in the callout since the review started, but the new sentence doesn't work: "Persepsi ilmuwan … cenderung **menyetujui**". Scientists agree, not their perceptions, and "krisis replikasi" appears twice. | "Sebagian besar ilmuwan sendiri mengakui bahwa krisis replikasi memang terjadi." |
| L651 / L665 | Two slides share the same heading and the same lead text. Quarto gives them duplicate IDs. | Retitle the second slide or merge the two. |
| L614 / L863 | Two "*Toolkit*" slides have near-identical titles. | Rename L863, e.g. "Tiga Kebiasaan untuk Dibawa Pulang", or fold it into the conclusion. |
| Front matter | There is no `lang: id`, so the date renders as "October 17, 2026". Also, the footer says "Pengantar Metasains" but the title says "Perkenalan Metasains". | Add `lang: id` (and optionally `date-format: "D MMMM YYYY"`), and use the same word in the footer and title. |

---

## 3. Accuracy: imprecise or overstated claims

- **L102, Bottesini et al. (2023).** The study did not measure whether journalists assume published Q1 papers replicate, and "Q1" never appears in it. Either drop the citation from this bullet, or rephrase it as "banyak jurnalis mengandalkan penanda status (jurnal bergengsi, status *peer review*)". The other Bottesini slides are accurate (N = 181, 8 vignettes, 4 factors, preregistered, sample size was the strongest factor).
- **L176, Tyner et al. (2026, SCORE).** The numbers are right, but:
  - "Dipilih acak" overstates it: the sampling was stratified random, but what got completed was limited by feasibility.
  - "Data *baru*" is not quite accurate: only 128 of 274 claims used new data; 146 used existing independent data.
  - The analysis groups disciplines into **6**, not 12. The "12" comes from the subfields in the press release.
  - It is 49% by paper, 55% by claim.
- **L244, Miske et al. (2026).** The 143 are **articles/datasets**, not claims. They are the subset of 600 sampled papers whose data were available (only 24% had data). About 74% were at least approximately reproducible.
- **L166, Errington et al. (2021).** The unit is "efek", not "klaim". The pooled 46% hides a split: 40% success for positive effects and 80% for null effects.
- **L183, "Decline effect".**
  - The "about half" figure comes from OSC (2015) and Camerer (2018). It covers *all* replications, not only successful ones.
  - SCORE's 0.25 → 0.10 is a 60% drop, not about half.
  - The linked Pietschnig (2019) paper is about decline over time in intelligence research, which is a different phenomenon from what the bullet describes. Consider framing the shrinkage as partly regression to the mean.
- **L281 (notes), Gelman & Loken.** "ketidakpastian sudah melekat pada realitas yang diteliti" misreads the idea. Forking paths means analysis choices *depend on the data*, so the real number of possible comparisons is far larger than reported, even without fishing. The PDF is dated 2013.
- **L402, van den Akker et al. (2024).** The study did not measure power. Preregistered studies *more often reported power analyses* and had larger samples.
- **L414, Stodden et al. (2018).** *Science*'s 2011 policy required data and code **on request**; it was not an open-data mandate. The 44% is the share of papers for which the authors supplied artifacts when asked.
- **L659, Wakefield.** Brian Deer's investigation began in **2004**, not 2009. The linked Times page is a 2025 book interview, not the original investigation.
- **L469 / L852–853, Jaring.id outcomes.**
  - The ethics sanction was **one** person at UMN, decided in 2023, *before* the 2024 report.
  - The Frontiers retractions (three Harun Achmad articles in April 2023, plus one Trias Mahmudiono article) also largely came before publication.
  - Present these as what the report documented, not as effects of the investigation. "Polanya sistematis" overstates what the article says ("disinyalir").
- **L60, ivermectin.** Erick Thohir said it "sudah keluar izin edarnya dari BPOM" while announcing it as a COVID therapy. He did not explicitly claim a COVID-19 indication. Also, production was halted partly by BPOM sanction (CPOB violations).
- **L450–453, L736, L854, Ariely.**
  - "18 dari 20 punya skor identik": more precisely, each of the 18 has a "twin" with identical scores in the same condition.
  - It was Wertenbroch who asked the journal to retract. Ariely said only that he would cooperate.
  - The editor (Vazire) said the journal is "considering next steps per COPE". So "jurnal sedang memproses retraksinya" is stronger than the source supports.
- **L260, Nuijten (2016).** The "half" is half of articles *that report NHST*, in 8 major journals. One in eight had a gross inconsistency.
- **L229, Chang & Li (2015).** The sample is narrow: macroeconomics papers using US GDP data, in a preliminary Fed discussion paper.
- **L110, terminology.** The definitions follow one convention (Turing Way, and the usage Barba prefers). Barba herself documents fields that use the terms the opposite way, and she doesn't define robustness. Also, "keandalan" is the standard Indonesian term for psychometric *reliability*; consider "kekokohan" for robustness.
- **L253, link.** The Business Insider (2018) link does not mention Reinhart & Rogoff. The Conversation piece does support the austerity point.
- **Minor.**
  - L635: Q1–Q4 are ranks, not "rata-rata sitasi".
  - L390: "Dampaknya" for Scheel (2021) implies causation that the study didn't test.
  - L955: Seglen (1997) is on pp. 498–502.
  - L676/L992: the Conversation topic is "Selisik Integritas **Akademis**", and the topic page doesn't describe it as a standing three-outlet collaboration.
  - L462 vs L976: the in-text "Jaring.id dkk." should match the reference entry "Somad dkk.".
  - L322: Merton should be cited as 1942/1973.
- **Could not verify (paywall or 403):** the Forbes April 2026 piece; Jones (2026) in *Nature*; the details of L673–676 attributed to Schapals et al. (2026) (the abstract doesn't name PubPeer or sleuths); the byline of the Rochmyaningsih (2018) piece; "GPT-6" (seems plausible).

**Verified as correct:** OSC 36%; Camerer 2016 (11/18) and 2018 (13/21); Baker (1,576; >70%, >50%, ~90%); Hardwicke (11/35; 25% → 78%); Crüwell (1/14); Claesen (25/27 deviated, 1 disclosed all); Scheel (44% vs 96%); Soderberg; Stodden (204, 44%, 26%); Fang 2012 (67.4%); Fang & Casadevall 2011; Van Noorden 2023 (all numbers, including the country rates); Reinhart & Rogoff (−0.1% vs 2.2%); RR in >300 journals; Permendikbudristek 39/2021 Pasal 9; the eucalyptus necklace details; BPOM and Harsen on ivermectin; Data Colada's d = 2.5 and the unrounded durations.

---

## 4. Logical flow

### High priority
1. **Metascience and open science come too late or are never defined.** "Apa Itu Metasains?" (L304) is roughly slide 16 of 50, in a talk titled "Perkenalan Metasains". "Sains terbuka" is in the title but is never defined. Section 02 is named "Cara Sains Mengoreksi Diri", but it's mostly about open-science practices; the self-correction idea only appears in the notes (Vazire & Holcombe, L757).
   Fixes:
   - Move "Apa Itu Metasains?" to right after Discussion 1.
   - Add a one-line definition of sains terbuka.
   - Rename section 02 to "Metasains dan Sains Terbuka: Bagaimana Sains Memeriksa dan Mengoreksi Diri".
   - Add a slide "Sains Mengoreksi Diri Hanya Jika Ada yang Memeriksa".
2. **The hook gives away the answer before Discussion 1.** L52 and L60 ("Padahal…", "BPOM membantah") and the callout at L64 are shown *before* you ask "apa yang Anda cek?". Show only the claims first, run the discussion, then reveal the corrections.
   The note at L79 says to revisit the answers in Bagian 03, but nothing there does this. Add a prompt at L530: "Buka kembali catatan diskusi pertama…". Optionally, add a short exercise applying the checklist to the eucalyptus necklace.
3. **Discussion 3 (L480) can't really be answered from what comes before.** Its premise ("jauh lebih lama") isn't supported, because neither case slide gives a timeline. The callout at L473–475 also gives away half the answer just before the question.
   Fixes:
   - Add timelines to both case slides (Ariely: 2002 → 2026; Jaring.id: 2024).
   - Move that callout into a debrief slide after the discussion.
   - Use that debrief to bridge to the "two paths" in section 03.
4. **Key terms are never explained for journalists.** These include *effect size* (and *d*, *r*), *p-hacking*, HARKing, *nilai p*, *paper mill*, Q1 and *impact factor* (used at L102 but defined at L635), *preprint*, and *statistical power* (sample size is the main Bottesini finding, but it is never linked to power). Add a short gloss in brackets at first use.

### Medium priority
- **The thought experiment and the terms slide are in opposite orders.** Q1 is replicability and Q2 is reproducibility (L100–101), but the terms slide defines reproducibility first. Robustness is defined but never used again; either tie it to Gelman & Loken, or move it to the notes.
- **Some slides are overloaded:**
  - "Hasil Coba Ulang" mentions SCORE twice.
  - "Apakah Praktik Sains Terbuka Ada Dampaknya?" has about 15 numbers and 7 citations.
  - "Contoh Kasus" and "Mengapa Krisis" are also too dense.
  - Split these, or move details (Errington 193→50, Naudet, Claesen) into the notes.
- **The cooking analogy shifts meaning.** In the reproducibility card, "resep" means the analysis; in the replicability card, it means the method. Pick one mapping (resep = prosedur, bahan = data, teknik = analisis).
  - The cards appear in a different order on L355 and L381.
  - The Devina slide (L341) asks the same question as L352.
- **"Mengapa Metasains Penting?" is three slides of images only.** The question is never answered in words. Merge them into one slide, or caption each with the Merton norm it shows.
- **Open science and fraud contradict each other across slides.** L429 and the conclusion (L899) say open science doesn't stop fraud. But Ariely was caught *because* the data were available. Say "tidak mencegah, tetapi membuat kecurangan lebih mudah terdeteksi".
- **"Prestise Jurnal Bukan Jaminan" (L625) is in the wrong place.** It continues the Bottesini findings, so move it before the checklist.
- **Checklist item 4 mixes things up.** Funding is a conflict-of-interest question; move it to item 2. The item also blurs the *pakar independen* (your source) with the *pemeriksa* (the sleuth).
- **The deck gives three different rules for naming the verifier.** "wajib" (L566), "hanya dengan persetujuan" (L753) and "Selalu sebut… (kalau bersedia)" (L887) conflict. Use one rule.
- **L693 asks "bagaimana agar kedua risiko diminimalisasi?" but no slide answers it explicitly.** Say which slides deal with Risiko 1 and which with Risiko 2.
- **The conclusion is missing pieces.** It doesn't mention metascience, the thesis that trust should be proportional to evidence (L682), or the before-publication practices.

### Timing
About 50 slides, with roughly 85–90 minutes of talking plus three 5–10-minute discussions, for **105–125 minutes** in total. That only fits a 2-hour slot if each discussion is held to 5 minutes. The reviewer's suggested cuts are in its full report; ask me if you want them.

---

## 5. Language (KBBI / EYD V)

### Clear errors
- **Typos:** L352 masakah → **masakan**; L390 metolodogis → **metodologis**; L422 "keterlibatan ~~yang~~ pihak lain"; L752 Perlu kah → **Perlukah**.
- **Non-standard forms:**
  - respon → **respons** (L147, L266, L749)
  - mempengaruhi → **memengaruhi** (L314, L628)
  - mengkoreksi → **mengoreksi** (L433)
  - sumberdaya → **sumber daya** (L314)
  - realitanya → **kenyataannya** (L433)
  - ekstrim → **ekstrem** (L636)
  - seringkali → **sering kali** (L750)
  - mempublikasi/dipublikasi → **-kan** (L270, L759)
  - pasca-publikasi → **pascapublikasi** (L618)
  - anti-sains → **antisains** (L675)
  - diminimalisasi → **diminimalkan** (L693)
- **Decimal points:** L176 `0.25`/`0.10` → `0,25`/`0,10`; L782 `67.4%` → `67,4%`.
- **Citation markers:** "Tyner, et al." (L176), "Miske, dkk." (L244) and "Stodden, dkk." (L414) should all be "X dkk.".
- **-nya with foreign words and numbers:** "*effect size*nya" (L183) → "*effect size*-nya". "26%nya" (L414) → "dan hanya 26% yang bisa direka ulang".
- **Missing words:**
  - "untuk": L462, L771, L826
  - "karena": L266 ("…tetapi **karena** respons…")
  - "pada": L271 ("bergantung **pada**")
  - "daripada": L812 (in place of "dari")
  - L272: "antara X ~~dengan~~ **dan** Y"
  - L742: delete "maka"
- **Broken sentences:**
  - L255: only one of the three items has a verb.
  - L253: grammatically it is the *countries* that "dikutip"; it should be the conclusion.
  - L402: "power" has nothing to compare against ("lebih tinggi daripada…").
  - L433: an incentive is compared with an activity.
  - L759: a time is compared with an announcement.
  - L834: "Minimalisasi" is a noun used as a command → "Minimalkan".
  - L450: "*d* = 2,5, 18 dari 20" is ambiguous → use semicolons.
  - L636: "artikel yang sangat ~~ekstrim~~ sering dikutip".
- **Heading capitalisation:**
  - "Sebagai" → "sebagai" (L137, L746)
  - "Pun" → "pun" (L218)
  - "Ketika" → "ketika" (L44)
  - L904 is in sentence case, while every other heading uses title case.

### Patterns to fix in one pass
1. **Dashes.** Four styles are mixed: ` - `, ` -- `, ` — ` and `—`. Use an en dash for ranges ("5–10 menit", L74/L290/L483).
2. **Foreign stem plus prefix.** Fix *ditrigger*, *Direcook*, *merecook*, *dipre-register* and *discroll*. Either hyphenate (as "di-*preregister*") or use Indonesian: dipicu, dimasak ulang, digulir.
3. **English abbreviations.** e.g., i.e. and tsb. → mis., yaitu, tersebut. Also "dsb)" → "dsb.)" at L429.
4. **Register.** Change "tapi" to "tetapi" (7×, including the labels "**Tapi:**"). Choose either "kalau" or "jika". Use fewer sentences that start with "Padahal" or "Tetapi".
5. **Italics.**
   - The headings Reproducibility, Replicability and Robustness are not italic, while their Indonesian glosses are.
   - Words left plain where the deck usually italicises them: "paper" (L141), "dataset" (L450), the journal name (L140).
   - "hydroxychloroquine" is plain while *ivermectin* is italic.
   - Change "*retraction*" and "*misconduct*" in the notes to retraksi and pelanggaran.
6. **"&" in running text.** Use "dan" (L252, L281, L446, L757, L314). Also cite "Simmons dkk., 2011" instead of listing all three names.
7. **Mixed variants of the same term:** pre-registration vs preregister; uji klinik vs uji klinis; imagetwin vs ImageTwin; "Psikologi" capitalised in running text (L143, L147).
8. **Reference list.**
   - File "The Center for Scientific Integrity" under C.
   - Add the missing article numbers (Bottesini, Schapals, Scheel).
   - The Merton chapter needs its editor or book details.
   - L1004: "or" → "atau".

---

*The three full reviewer reports, with every finding, are available on request.*

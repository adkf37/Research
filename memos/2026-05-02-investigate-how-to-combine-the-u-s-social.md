# Combining the U.S. Social Security Card and Passport into a National ID from Birth

**Date:** 2026-05-02  
**Output Type:** research_memo  
**Source Prompt:** Investigate how to combine the U.S. Social Security card and passport into a single national ID that everybody has from birth. What pilot programs have looked at this? What hurdles? Let's also start to think about cost?

---

## Executive Summary

The short answer is that the United States **could not realistically “merge” the Social Security card and passport into a single national ID just by administrative coordination**. It would need **new federal legislation**, major state-federal agreements on birth and vital-records data, and a policy choice about whether the new credential is mainly for **citizenship proof, service access, travel, employment verification, or all of the above**. Those functions are currently split on purpose. The Social Security Administration itself says a Social Security card is **not** proof of identity or citizenship, while the passport system is built around a higher-proofing citizenship and travel credential ([SSA SSN guidance](https://www.ssa.gov/ssnumber/); [26 U.S.C. § 6039E / implementing regulation](https://www.ecfr.gov/current/title-26/chapter-I/subchapter-F/part-301/subpart-ECFR1b5d05d4bfe19f9/subject-group-ECFR2bb42ef5f1a3a92/section-301.6039E-1)).

The closest U.S. “pilots” are **partial integration programs**, not a true national-ID pilot. The strongest analogue is **Enumeration at Birth (EAB)**, which began as a 1987 pilot in New Mexico, Iowa, and Indiana and now issues roughly **99% of infant SSNs** through hospital birth registration. Other important analogues are **Enumeration at Entry** for some immigrants, **Electronic Verification of Vital Events (EVVE)** for checking birth/death records, the **passport card / Western Hemisphere Travel Initiative** rollout, **enhanced driver’s licenses**, and NIST’s **NSTIC identity pilots** for digital identity. Together they show that the government can link identity systems in pieces; they do **not** show that the United States has tested a universal federal identity card from birth ([SSA EAB FAQ](https://www.ssa.gov/faqs/en/questions/KA-10041.html); [SSA OIG EAB/EAE report](https://oig.ssa.gov/assets/uploads/A-08-14-34124.pdf); [NAPHSIS EVVE](https://www.naphsis.org/evve/); [DHS REAL ID](https://www.dhs.gov/real-id); [DHS Enhanced Driver’s Licenses](https://www.dhs.gov/enhanced-drivers-licenses-what-are-they); [NIST NSTIC pilots](https://csrc.nist.gov/pubs/ir/8054/upd1/final)).

The biggest hurdles are **federalism, privacy, and functional mismatch**. Birth records are state-run; passports are federal; Social Security numbers were never designed to be a secure national authenticator; and a passport-like credential has renewal, citizenship, photo, and fraud-control demands that do not fit cleanly with universal newborn issuance. A from-birth national ID would also need an answer for **children born abroad**, whose foundational citizenship document is a **Consular Report of Birth Abroad**, not a state birth certificate ([State CRBA guidance](https://travel.state.gov/content/travel/en/international-travel/while-abroad/birth-abroad.html)). Institutional analyses going back to GAO and CRS warn that national ID systems create large privacy, surveillance, and database-governance risks even if they may also reduce some forms of fraud ([GAO-03-982T](https://www.gao.gov/assets/gao-03-982t.pdf); [CRS RS21137 archive](https://www.everycrsreport.com/reports/RS21137.html)).

On cost, the evidence supports an **order-of-magnitude judgment, not a precise budget**. There is no official federal estimate for a combined SSN-passport-at-birth ID system. But the best analogues imply **multi-billion-dollar startup and operating costs**. DHS estimated **REAL ID** implementation at about **$9.9 billion over ten years** in its 2008 final rule, and GAO testified in 2003 that a national identification card system would cost **billions of dollars**. Because a true birth-to-death federal ID would require not just card issuance but also **vital-record modernization, secure lifecycle management, foreign-birth workflows, legacy-population enrollment, and stronger privacy/cybersecurity controls**, it would likely cost **at least** in that general range and possibly more ([REAL ID final rule cost discussion, 73 Fed. Reg. 5272, 5324-29](https://www.alston.com/-/media/files/insights/publications/2008/05/dhss-final-regulations-implementing-title-ii-of-th/files/real-id-final/fileattachment/real-id-final.pdf); [GAO-03-982T](https://www.gao.gov/assets/gao-03-982t.pdf); [CDC NVSS modernization](https://www.cdc.gov/nchs/nvss/modernization.htm)).

## Question

How could the United States combine Social Security and passport-style identity documentation into a single national ID issued from birth, what pilots or analogous programs have explored parts of that model, what major hurdles would such a policy face, and what is the early evidence on cost?

## What matters most

1. **There is no U.S. pilot for a universal national ID from birth.** The relevant evidence comes from **partial pilots and adjacent systems**, especially EAB, EAE, EVVE, REAL ID, enhanced driver’s licenses, passport cards, and NSTIC digital-identity pilots.
2. **The core policy challenge is functional mismatch.** Social Security numbers are administrative identifiers; passports are high-proofing citizenship and travel documents. Combining them changes the legal and operational purpose of both systems.
3. **State vital records are the choke point.** A birth-to-ID model only works if state birth/death systems, federal citizenship workflows, and replacement/amendment processes become more interoperable and more trusted.
4. **Privacy and federalism are not side issues.** They are likely the main political barriers, as earlier national-ID and REAL ID debates show.
5. **Cost will almost certainly be in the billions.** The available analogues show that even narrower identity-standardization efforts are expensive; a true national ID from birth would be broader still.

## Analysis

### 1. Current U.S. identity architecture

The first obstacle is conceptual. The United States does not have one general-purpose identity credential because it uses **different documents for different legal functions**.

- The **Social Security number** is primarily a tax and benefits identifier. SSA explicitly says the card is **not** an identity document and does **not** establish citizenship or immigration status ([SSA SSN guidance](https://www.ssa.gov/ssnumber/)).
- The **passport system** is a citizenship and travel-credential system with higher documentary proofing. Federal law and regulations require passport applicants to provide a taxpayer identification number, usually an SSN, which means the passport system already leans on the SSN system rather than replacing it ([26 U.S.C. § 6039E / implementing regulation](https://www.ecfr.gov/current/title-26/chapter-I/subchapter-F/part-301/subpart-ECFR1b5d05d4bfe19f9/subject-group-ECFR2bb42ef5f1a3a92/section-301.6039E-1)).
- For people **born abroad to U.S. citizens**, the foundational citizenship document is a **Consular Report of Birth Abroad (CRBA)**, not a state birth certificate, and it still does not automatically function as a passport ([State CRBA guidance](https://travel.state.gov/content/travel/en/international-travel/while-abroad/birth-abroad.html)).

This matters because “combine the Social Security card and passport” is not just a card-design problem. It requires deciding whether the new document would be:

1. a **citizenship credential**,
2. a **general identity credential**,
3. a **service-access credential**,
4. a **domestic travel / employment-verification credential**,
5. or all of the above.

Those choices drive the proofing burden, renewal cycle, data fields, privacy rules, and agency ownership.

### 2. Pilot programs and analogues

The best answer to “what pilot programs have looked at this?” is that **the U.S. has tested pieces of the stack, not the whole model**.

**Enumeration at Birth (EAB)** is the clearest precedent. SSA says EAB began as a **pilot in 1987 in New Mexico, Iowa, and Indiana** and now handles about **99% of infant SSN assignments** by linking state birth registration to SSA issuance ([SSA EAB FAQ](https://www.ssa.gov/faqs/en/questions/KA-10041.html)). That is important because it proves one foundational point: the government can issue an identity-related federal credential at birth through a hospital/vital-records workflow.

But EAB also highlights the limits of the analogy. It works because an SSN is just a unique identifier plus a mailed paper card. It does **not** require a photo, biometrics, evidence of future travel eligibility, or repeated in-person renewals. In other words, EAB shows that the **birth-registration link** is feasible; it does **not** show that a passport-like credential can be universalized at birth with the same ease.

**Enumeration at Entry (EAE)** is a second relevant analogue. It lets some lawful permanent residents request SSNs during the immigration-visa process, with State, DHS, and SSA sharing data so the card can be issued after arrival. That shows another identity-integration path: federal agencies can sometimes pre-stage identity issuance when the upstream legal-status event is trustworthy and standardized ([SSA EAE FAQ](https://www.ssa.gov/faqs/en/questions/KA-10040.html)).

**EVVE and vital-records modernization** are the infrastructure analogue. NAPHSIS’s **Electronic Verification of Vital Events** gives authorized agencies a way to verify birth and death records against state records, and CDC’s NVSS modernization effort aims at more modern, interoperable vital-statistics systems ([NAPHSIS EVVE](https://www.naphsis.org/evve/); [CDC NVSS modernization](https://www.cdc.gov/nchs/nvss/modernization.htm)). GAO has repeatedly treated this missing nationwide verification layer as a central weakness in both SSN and passport issuance. In 2005, GAO recommended moving toward electronic verification of birth certificates for child SSN issuance; in 2009 it showed how passport issuance remained vulnerable when staff could not verify birth certificates in real time ([GAO-05-115](https://www.gao.gov/products/gao-05-115); [GAO-09-447](https://www.gao.gov/assets/gao-09-447.pdf); [GAO-09-681T](https://www.gao.gov/assets/gao-09-681t.pdf)).

**Passport cards, WHTI, and enhanced driver’s licenses** are the best secure-credential analogues. The passport card created a lower-cost, wallet-sized federal citizenship/identity document for limited border use, while enhanced driver’s licenses show that Washington can certify state-issued documents that also attest citizenship for certain border crossings ([State passport card page](https://travel.state.gov/content/travel/en/passports/need-passport/card.html); [CBP WHTI](https://www.cbp.gov/travel/us-citizens/western-hemisphere-travel-initiative); [DHS Enhanced Driver’s Licenses](https://www.dhs.gov/enhanced-drivers-licenses-what-are-they)). But these are targeted travel/security credentials for limited populations, not universal birth-issued IDs.

**NSTIC pilots** are the digital analogue. NIST’s pilots under the National Strategy for Trusted Identities in Cyberspace were meant to catalyze interoperable digital identity solutions, but they were explicitly designed as a **voluntary identity ecosystem**, not a compulsory national ID ([NIST NSTIC pilots](https://csrc.nist.gov/pubs/ir/8054/upd1/final)). That distinction matters because it reflects a long-standing U.S. preference for federated and sectoral identity systems over a mandatory single credential.

The most defensible synthesis is therefore: **the United States has piloted the plumbing for a national ID, but not the national ID itself**.

### 3. Legal, political, and implementation hurdles

The first hurdle is **federalism**. Birth certificates are issued and amended by states; passport documents are federal; driver licensing is mostly state-based; Social Security is federal. A unified ID would therefore need either:

- federal preemption plus new federal administrative machinery,
- a cooperative federal-state regime with standardization requirements,
- or a narrower federal credential layered on top of state vital records.

That state-federal tension is a recurring theme in national-ID and REAL ID debates. CRS and GAO both emphasize that a national identification card would require clear statutory authority, explicit privacy design, and agreement on how much state data infrastructure gets absorbed into a federal system ([GAO-03-982T](https://www.gao.gov/assets/gao-03-982t.pdf); [CRS RS21137 archive](https://www.everycrsreport.com/reports/RS21137.html)).

The second hurdle is **privacy and surveillance risk**. A merged ID would create a richer, more central identity record than either the current SSN card or passport alone. That can help with anti-fraud and service delivery, but it also increases the value of the database to attackers and the risk of “mission creep,” where the credential becomes necessary for more and more activities. That concern is not speculative; it has been central to the U.S. national-ID debate for decades, and it was a major line of resistance to REAL ID as well ([GAO-03-982T](https://www.gao.gov/assets/gao-03-982t.pdf); [CRS RS21137 archive](https://www.everycrsreport.com/reports/RS21137.html)).

The third hurdle is **lifecycle management**. A birth-issued SSN works partly because the number does not need to change as the child grows. A passport-like credential is harder. A newborn cannot supply a durable photo or useful biometrics for long-term authentication, which means a serious national ID from birth would still need:

1. an initial registration event at birth,
2. later age-based photo or biometric capture,
3. replacement and re-verification workflows,
4. name and status-change processing,
5. and a strong death-record linkage to reduce posthumous fraud.

That is operationally much closer to running a universal passport-plus-civil-registry system than to mailing a Social Security card.

The fourth hurdle is **coverage complexity**. The system must decide how to treat:

- citizens born in U.S. hospitals,
- home births and delayed registrations,
- U.S. citizens born abroad with CRBAs,
- adopted children,
- lawful noncitizens,
- and people whose birth records are incomplete or later amended.

The more universal the credential, the more politically salient these edge cases become.

The fifth hurdle is **institutional trust**. Current evidence suggests the United States has managed identity modernization best when it adds one narrow layer at a time—EAB, EVVE, passport cards, REAL ID compliance, digital pilots—rather than when it proposes a fully unified identity architecture.

### 4. Early cost considerations

There is **no official score** for a combined “Social Security + passport + national ID from birth” system. That is an important finding in itself.

Still, the available analogues give a useful cost frame:

- DHS’s 2008 **REAL ID** final rule estimated roughly **$9.9 billion over ten years** in implementation costs for a narrower identity-standardization effort focused on state-issued licenses and IDs ([73 Fed. Reg. 5272, 5324-29](https://www.alston.com/-/media/files/insights/publications/2008/05/dhss-final-regulations-implementing-title-ii-of-th/files/real-id-final/fileattachment/real-id-final.pdf)).
- GAO testified in 2003 that a national identification card system would cost **billions of dollars**, depending on technology, enrollment, and operating design ([GAO-03-982T](https://www.gao.gov/assets/gao-03-982t.pdf)).
- The **passport card** itself is a useful reminder that even limited secure credentials have meaningful per-card and processing costs; State currently prices it separately from the passport book rather than treating it as negligible overhead ([State passport card page](https://travel.state.gov/content/travel/en/passports/need-passport/card.html)).
- CDC and NAPHSIS modernization materials suggest that **vital-records modernization is an ongoing capital and governance project**, not a one-time switch flip ([CDC NVSS modernization](https://www.cdc.gov/nchs/nvss/modernization.htm); [NAPHSIS vital records modernization](https://www.naphsis.org/vital-records-modernization/)).

For a genuine from-birth national ID, the cost drivers would include at least:

1. **new federal IT integration** across SSA, State, DHS, IRS, and state vital-records offices;
2. **credential production and distribution**, whether physical, digital, or both;
3. **age-based refreshes** for photos or biometrics;
4. **privacy, cybersecurity, and oversight controls**;
5. **retroactive enrollment** of the entire existing population, not just newborns;
6. **exception handling** for people born abroad, missing records, or contested status.

That suggests a practical policy conclusion: if Congress wanted to explore this seriously, it would first need a **formal cost model** and likely a staged approach rather than a one-shot national rollout.

### 5. Counterarguments and contradictory evidence

There are real arguments **for** a single national ID. Fragmented U.S. identity systems create fraud opportunities, place burdens on individuals to assemble multiple documents, and make digital-service access harder than it needs to be. EAB is strong evidence that when the upstream event is standardized, the U.S. can issue identity-linked credentials efficiently at scale. EVVE and other verification systems show that better backend verification can reduce fraud and administrative friction.

There are also strong arguments **against** assuming a merged credential would solve more than it creates. The same centralization that can reduce fraud can also magnify the consequences of error, exclusion, or breach. GAO’s passport investigations show the government still struggles with foundational document verification in some workflows, which suggests that “make one stronger national card” is not a substitute for fixing the underlying registries ([GAO-09-447](https://www.gao.gov/assets/gao-09-447.pdf); [GAO-09-681T](https://www.gao.gov/assets/gao-09-681t.pdf)).

The contradictory lesson from recent U.S. history is that **incremental identity integration often works**, but **comprehensive national-ID politics often do not**. REAL ID survived, but only after long delays, state resistance, and a narrower practical role than many people first assumed. NSTIC produced useful pilots, but only in a voluntary ecosystem rather than a mandatory federal credential. That evidence favors gradualism over a clean-sheet national-ID replacement.

## Source ledger

- **SSA Enumeration at Birth materials and OIG reporting** — the most important evidence on what the U.S. has actually done at birth scale; shows the strongest real pilot analogue and its limits. <https://www.ssa.gov/faqs/en/questions/KA-10041.html>; <https://oig.ssa.gov/assets/uploads/A-08-14-34124.pdf>
- **GAO reports on SSNs, passports, and national ID** — central for hurdles and costs because they connect identity issuance, fraud vulnerabilities, and national-ID tradeoffs in official oversight documents. <https://www.gao.gov/assets/gao-03-982t.pdf>; <https://www.gao.gov/products/gao-05-115>; <https://www.gao.gov/assets/gao-09-447.pdf>; <https://www.gao.gov/assets/gao-09-681t.pdf>
- **State Department / Treasury rules on passport identity proofing** — important because they show the passport system already depends on SSNs and separate citizenship proofing, which is why a merger is nontrivial. <https://www.ecfr.gov/current/title-26/chapter-I/subchapter-F/part-301/subpart-ECFR1b5d05d4bfe19f9/subject-group-ECFR2bb42ef5f1a3a92/section-301.6039E-1>; <https://travel.state.gov/content/travel/en/passports/need-passport/card.html>; <https://travel.state.gov/content/travel/en/international-travel/while-abroad/birth-abroad.html>
- **DHS / CBP / REAL ID materials** — best official analogue for a politically contested identity-standardization project with real implementation costs. <https://www.dhs.gov/real-id>; <https://www.cbp.gov/travel/us-citizens/western-hemisphere-travel-initiative>; <https://www.dhs.gov/enhanced-drivers-licenses-what-are-they>; <https://www.alston.com/-/media/files/insights/publications/2008/05/dhss-final-regulations-implementing-title-ii-of-th/files/real-id-final/fileattachment/real-id-final.pdf>
- **NAPHSIS / CDC / NIST materials** — important for the infrastructure and digital-identity layers: vital-record verification, modernization, and voluntary digital identity pilots. <https://www.naphsis.org/evve/>; <https://www.cdc.gov/nchs/nvss/modernization.htm>; <https://csrc.nist.gov/pubs/ir/8054/upd1/final>
- **CRS national-ID analysis** — useful institutional synthesis for the recurring legal and civil-liberties objections that any national-ID proposal would have to overcome. <https://www.everycrsreport.com/reports/RS21137.html>

## Claims check

- **Weak / unsupported:** there is **no direct U.S. pilot** for a single national ID that combines Social Security and passport functions for everyone from birth. The memo therefore relies on **analogues**, not a one-to-one precedent.
- **Uncertain:** there is **no official comprehensive cost estimate** for the exact policy proposed here. The memo uses REAL ID and GAO national-ID estimates only as scale markers.
- **Contested:** whether a merged national ID would materially reduce fraud more than backend verification improvements alone is not settled by the available evidence.
- **Contested:** whether biometric capture should happen at birth, later in childhood, or only on renewal is a design issue the existing U.S. evidence base does not resolve cleanly.
- **Important caveat:** a national ID “for everybody from birth” must still answer whether “everybody” means only citizens, all lawful residents, or all people recorded in U.S. civil registries. The sources reviewed do not yield a single obvious legal design.

## References

1. Social Security Administration, **Social Security Number and Card**. <https://www.ssa.gov/ssnumber/>
2. Social Security Administration, **What is Enumeration at Birth and how does it work?** <https://www.ssa.gov/faqs/en/questions/KA-10041.html>
3. SSA Office of Inspector General, **Enumeration at Birth and Enumeration at Entry Programs**. <https://oig.ssa.gov/assets/uploads/A-08-14-34124.pdf>
4. Social Security Administration, **What is Enumeration at Entry and how does it work?** <https://www.ssa.gov/faqs/en/questions/KA-10040.html>
5. Government Accountability Office, **National Identification Cards (GAO-03-982T)**. <https://www.gao.gov/assets/gao-03-982t.pdf>
6. Government Accountability Office, **Social Security Administration: Actions Needed to Strengthen Processes for Issuing Social Security Numbers to Children (GAO-05-115)**. <https://www.gao.gov/products/gao-05-115>
7. Government Accountability Office, **State Department: Undercover Tests Reveal Significant Vulnerabilities in Passport Issuance Process (GAO-09-447)**. <https://www.gao.gov/assets/gao-09-447.pdf>
8. Government Accountability Office, **Significant Vulnerabilities in the Passport Issuance Process (GAO-09-681T)**. <https://www.gao.gov/assets/gao-09-681t.pdf>
9. 26 C.F.R. § 301.6039E-1, **Information reporting by passport applicants**. <https://www.ecfr.gov/current/title-26/chapter-I/subchapter-F/part-301/subpart-ECFR1b5d05d4bfe19f9/subject-group-ECFR2bb42ef5f1a3a92/section-301.6039E-1>
10. U.S. Department of State, **Get a Passport Card**. <https://travel.state.gov/content/travel/en/passports/need-passport/card.html>
11. U.S. Department of State, **Consular Report of Birth Abroad**. <https://travel.state.gov/content/travel/en/international-travel/while-abroad/birth-abroad.html>
12. Department of Homeland Security, **REAL ID**. <https://www.dhs.gov/real-id>
13. U.S. Customs and Border Protection, **Western Hemisphere Travel Initiative**. <https://www.cbp.gov/travel/us-citizens/western-hemisphere-travel-initiative>
14. Department of Homeland Security, **Enhanced Driver’s Licenses: What Are They?** <https://www.dhs.gov/enhanced-drivers-licenses-what-are-they>
15. Department of Homeland Security, **REAL ID final rule cost discussion** (73 Fed. Reg. 5272, 5324-29). <https://www.alston.com/-/media/files/insights/publications/2008/05/dhss-final-regulations-implementing-title-ii-of-th/files/real-id-final/fileattachment/real-id-final.pdf>
16. NAPHSIS, **Electronic Verification of Vital Events (EVVE)**. <https://www.naphsis.org/evve/>
17. Centers for Disease Control and Prevention, **Modernizing the National Vital Statistics System**. <https://www.cdc.gov/nchs/nvss/modernization.htm>
18. NAPHSIS, **Vital Records Modernization**. <https://www.naphsis.org/vital-records-modernization/>
19. National Institute of Standards and Technology, **NSTIC Pilots: Catalyzing the Identity Ecosystem (NIST IR 8054)**. <https://csrc.nist.gov/pubs/ir/8054/upd1/final>
20. Congressional Research Service archive, **National Identification Cards: Legal Issues (RS21137)**. <https://www.everycrsreport.com/reports/RS21137.html>

## Recommended follow-ups

1. Commission a **formal cost model** for three options: backend-only integration, optional federal smart credential, and mandatory national ID from birth.
2. Do a **legal design memo** on scope: citizens only, all lawful residents, or broader civil-registry coverage.
3. Map the **exception pathways** in detail: births abroad, delayed birth registration, adoption, name changes, and deaths.
4. Assess whether the best first move is **not** a new card, but nationwide **vital-record verification and lifecycle modernization**.
5. If policymakers still want a pilot, test a **narrow, voluntary federal digital identity linked to verified birth records** before attempting a universal compulsory credential.

## Decision-oriented conclusion

The best evidence suggests that a U.S. “single national ID from birth” is **more plausible as a long, staged state-capacity project than as an immediate merger of the Social Security card and passport**. A reader should believe three things. First, the U.S. already has some of the necessary plumbing—especially EAB, EVVE, and passport/SSN linkages—but **not** a tested model for a universal credential. Second, the biggest barriers are not card design; they are **federalism, privacy, lifecycle management, and cost**. Third, if policymakers want to move in this direction, the prudent next step is to strengthen **vital-record verification and interoperable identity infrastructure first**, then evaluate whether a voluntary or limited federal credential adds enough value to justify the political and fiscal cost of a true national ID.

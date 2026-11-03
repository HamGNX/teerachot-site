# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS (`index.html`, `style.css`), no framework or build step. Must stay that way: plain files served as-is at teerachot.com.

## Users

Primary: recruiters and engineering managers hiring for full-time software/systems roles. They usually arrive from a resume, LinkedIn, or GitHub link, scan quickly, and decide whether to open the resume or make contact. Many of them are not technical (HR, talent teams), so the site must make sense without engineering jargon.

Teerachot is currently employed and open to offers, so the site is a standing professional presence rather than an active job application.

Secondary: Thai-speaking visitors, served by a full Thai version of the site.

## Product Purpose

Personal portfolio for Teerachot Khusuwan. It exists to show a hiring reader, within a short scan, what Teerachot can build and to make getting in touch or opening the resume effortless. Success means a qualified reader opens the resume or gets in touch.

## Positioning

A broad systems engineer: range is the point. The work moves from hardware (Jetson Nano, Arduino, Raspberry Pi) through security detection (SQLi detection, rootkit/bootkit detection with TEE–TPM) and applied ML (OCT image segmentation) up to web apps and automation. Security is one strong thread, not the whole identity. Peer-reviewed publications back the claim with evidence.

## Operating Context

- Visitors read on desktop and phone, often in a quick screening pass.
- The resume PDF and GitHub profile are the main follow-through destinations.
- The site is the canonical link behind the resume and LinkedIn.

## Capabilities and Constraints

- Sections today: hero, About, Selected Projects, Publications, Technical Stack, Contact.
- Required: a full English/Thai language toggle covering the whole site, delivered without a build step.
- Contact links are professional only: email, GitHub, LinkedIn. The Facebook link is to be removed.
- Copy describing Teerachot as a student seeking internships is outdated and must be updated to "employed, open to offers".
- Open decisions: current role and company (not confirmed; do not state one), Thai translation copy (to be supplied or approved by Teerachot), and whether "Class 2026" stays.

## Brand Commitments

- Name: Teerachot Khusuwan; monogram "TK"; domain teerachot.com.
- Education: Computer Engineering, Sirindhorn International Institute of Technology (SIIT), Thammasat University, class of 2026.
- Location: Pathum Thani, Thailand.
- Tone (user-stated, standing): professional and approachable for non-technical readers; never nerdy or in-joke. No hacker, terminal, or hardware-part costumes.

## Evidence on Hand

- Resume: `Teerachot_Khusuwan_Resume2026.pdf`.
- Publications (real, linked):
  - "Rootkit and Bootkit Detection Using TEE–TPM Architecture with Machine Learning and Blockchain Verification", KST 2026, IEEE, DOI 10.1109/KST67832.2026.11432384.
  - "Automated Detection and Segmentation of Choroidal Neovascularization in OCT Using Deep Learning", Science & Technology Asia 30(3), 2025.
- Projects: SQLIX (injection detection), Taek8 (TFT tracker Discord bot), Auto Vision Screening (hospital prototype), Clinic Appointment System.
- GitHub: github.com/HamGNX. LinkedIn: linkedin.com/in/teerachot-khusuwan.
- Absent, and not to be fabricated: project screenshots or demos, testimonials, employer name, metrics or impact numbers.

## Product Principles

1. Show range through real work: every claim of breadth points to a project, publication, or tool actually used.
2. Respect the screening reader: who Teerachot is, what they build, and how to get in touch should be clear within one scroll.
3. Evidence over adjectives: publications and shipped projects carry the credibility, not self-description.
4. Two languages count equally: Thai is a full version, not an afterthought.
5. Stay plain files: anything added must work as static HTML/CSS with minimal script.

## Accessibility & Inclusion

Keep the existing skip link, landmarks, and keyboard focus. The language toggle must set `lang` correctly per language and let screen readers and keyboard users switch.

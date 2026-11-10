# Community Deception Techniques: Coordinated Social Engineering in WhatsApp Group Scams
 
A mixed-methods case study of how coordinated groups of fake accounts manufacture trust in cryptocurrency investment scams on WhatsApp.
 
**Authors:** Derek Hansen, Benjamin Schooley, Ryan Rushton, Diego R. Orozco del Cid, Zane Wong, Jonathan Houston
**Affiliation:** Brigham Young University, Ira A. Fulton College of Engineering, Provo, UT
**Funding:** Supported in part by NSF #2336409
 
---
 
## Overview
 
Most research on social engineering focuses on a single scammer persuading a single victim. This project looks at something different: **how a network of fraudulent accounts works together to fabricate an entire investment community.**
 
We studied two WhatsApp groups run by the "GateMix" cryptocurrency mixing scam (528 messages, 15-16 fake participant accounts per group). Using qualitative thematic analysis, temporal analysis, and social network analysis (SNA), we examined the social roles, interaction patterns, and persuasion strategies used to create the illusion of a thriving community.
 
We introduce the concept of **community deception techniques**: manipulation strategies that depend on coordinated interaction among multiple fraudulent accounts rather than the actions of one scammer.
 
## Key Findings
 
- **Complementary roles.** Fake accounts fall into four roles: *admin*, *expert*, *newcomer*, and *peripheral*. Newcomers ask questions, experts answer them, and some newcomers gradually "become" experienced investors, modeling the path a real victim is meant to follow.
- **Dense, reciprocal networks.** The two groups showed strikingly similar structure (network density of 0.26 and 0.45; 44% and 78% of edges reciprocated), which gives an impression of an active community with frequent back-and-forth.
- **Rapid, steady activity.** Median time between posts was about 3-4 minutes, with posting concentrated in U.S. waking hours.
- **Suspiciously uniform text.** Messages share a polished, promotional voice, with no slang, emojis, misspellings, or disagreements, and none were duplicated. This suggests an LLM or template was used to generate them.
- **Six community deception techniques** (see table below), each of which requires multiple participants to carry out.
- **Detection potential.** Community-level signals (role structure, reciprocity, response times, and tone consistency) could complement message-level scam detection.
### Community Deception Techniques
 
| Technique | Summary |
|---|---|
| Q&A Consensus Building | Newcomers ask questions; several "experts" give consistent advice recommending the scam platform. |
| Community Exposure | Many members share success stories, profit screenshots, and withdrawal evidence. |
| Resolved Skepticism | One member voices doubt and another resolves it. |
| Collective Validation of Authorities | Multiple members praise and thank managers or experts. |
| Behavioral Modeling | Members publicly take increasingly committed actions (more orders, more money, inviting friends). |
| Community Belonging | Members welcome newcomers, celebrate milestones, and reinforce a shared group identity. |
 
## Methods
 
| Approach | Details |
|---|---|
| Data collection | Authors were added to two GateMix WhatsApp groups (Group 742 and Group 8808) and downloaded all 528 messages, plus images where available, timestamps, and usernames, before WhatsApp suspended the groups. |
| Social network analysis | Performed in [NodeXL](https://www.smrfoundation.org/nodexl/) using the WhatsApp importer. Nodes are accounts; directed, weighted edges are sequential posts. Metrics include in/out-degree, density, and reciprocity. |
| Temporal analysis | Post frequency over time and the median, mean, and standard deviation of time between same-day posts. |
| Qualitative analysis | Two authors independently coded account roles and inductively developed the community deception techniques through thematic analysis. |
 
## Ethics and Data
 
The groups appeared to be a coordinated scam, but participant identities and roles could not be independently verified, and messages may have been written by humans or AI agents. To protect privacy:
 
- Usernames, profile photos, phone numbers, and other identifying details were replaced or obscured (the "GateMix" brand name is retained).
- Screenshots were edited to remove identifying information.
- WhatsApp has removed both groups.
> **Note:** [Describe here what, if anything, this repository shares: e.g., anonymized data, analysis scripts, figures. Update this section before publishing.]
 
## Repository Contents
 
> [Fill in to match your repository. Example layout:]
 
```
.
├── paper/        # PDF of the paper
├── figures/      # Network graphs, heatmaps, and architecture diagram
├── analysis/     # Scripts or notebooks for temporal / network analysis
└── README.md
```
 
## Citation
 
If you use or reference this work, please cite:
 
```bibtex
@inproceedings{hansen2026community,
  title     = {Community Deception Techniques: Coordinated Social Engineering in WhatsApp Group Scams},
  author    = {Hansen, Derek and Schooley, Benjamin and Rushton, Ryan and
               Orozco del Cid, Diego R. and Wong, Zane and Houston, Jonathan},
  booktitle = {[Venue]},
  year      = {2026}
}
```

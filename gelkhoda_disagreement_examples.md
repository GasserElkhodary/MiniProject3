# Disagreement Examples — gelkhoda & sbombry1

Parties: Gasser Elkhodary (gelkhoda) and Samuel Bombrys (sbombry1). Each of us validated the other's ten MiniProject2 projects across five fields (100 comparisons in total, 28 disagreements). All 28 are listed in `gelkhoda_disagreement_resolution.csv`; five representative cases follow.

## Example 1 — arfc/pride (ActivityPattern)
**Author (sbombry1):** declining  
**Validator (gelkhoda):** stopped  
**Evidence:** 736 commits in 2020 and 236 in 2021, then zero in 2022–2023. After the gap there are only a `.gitattributes` file and merge commits for a paper branch (2024–Feb 2025).  
**Discussion:** The decline is real, but the codebook defines "stopped" as activity that ceased with no sign of recovery, which better fits a project whose last real development was in 2021.  
**Resolution:** ValidatorKept → **stopped**. The author's WhyRecovered text ("Milestone hit didn't stop development") also contradicted HasRecovered = No, so it was set to N/A.

## Example 2 — gabinsane/multimodal-vae-comparison (Currentstatus)
**Author (sbombry1):** Inactive  
**Validator (gelkhoda):** Active  
**Evidence:** Last commits are on 2025-05-19 ("vilanro-trimodal added", "bug fixes"), after the 2025-04-01 cutoff.  
**Discussion:** The author judged the project dead from the plot, which is fair in spirit, but the codebook rule is purely date-based. We noted that HasRecovered = No and Currentstatus = Active can both be true: a one-day burst counts as recent activity but not as a recovery.  
**Resolution:** ValidatorKept → **Active**. tompollard/tableone was corrected the same way (v0.9.6 released Feb 2026).

## Example 3 — statistikat/VIM (WhyRecovered)
**Author (sbombry1):** Gap was scheduled.  
**Validator (gelkhoda):** New contributor began developing the vimpute imputation framework.  
**Evidence:** From 2025-04-11, Eileen Vattheuer commits "helpers", "vimpute", "vig" and xgboost threading. Nothing in commits, README or issues indicates a planned pause.  
**Resolution:** ValidatorKept. A recovery reason should be visible in the commits or issues, not assumed.

## Example 4 — FairRootGroup/FairRoot (WhyRecovered)
**Author (sbombry1):** Simply focused with Release.  
**Validator (gelkhoda):** Resumed with repository maintenance (stale-issue workflow) and macOS build fixes.  
**Evidence:** The last pre-gap commits are "Bump v19.0.0" / "Merge v19.0.0". The first post-gap commits are "workflow: Mark issues/PRs as stale" and "fix(build): Properly pass CMAKE_OSX_SYSROOT".  
**Resolution:** Compromise → "Post-release lull (v19.0.0) ended by repository maintenance and build fixes". The author explained the gap and the validator explained the restart. tableone, nexpy and posteriordb were resolved the same way.

## Example 5 — sakov_enkf-c (RecentThemes; author gelkhoda, validator sbombry1)
**Author (gelkhoda):** Release:Other  
**Validator (sbombry1):** Release:Bug fixes  
**Evidence:** All ten most recent commits are version tags (v2.39.2 … v2.40.0) with no other message content.  
**Resolution:** Compromise → **Release** only. When every commit falls in one theme, neither second theme is supported.

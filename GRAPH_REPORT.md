# Graph Report - .  (2026-07-06)

## Corpus Check
- Large corpus: 4057 files ┬À ~3,274,290 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 161 nodes · 206 edges · 20 communities (15 shown, 5 thin omitted)
- Extraction: 79% EXTRACTED · 21% INFERRED · 0% AMBIGUOUS · INFERRED: 43 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_E-Invoicing System (APOL)|E-Invoicing System (APOL)]]
- [[_COMMUNITY_INSEAD Application Programmes|INSEAD Application Programmes]]
- [[_COMMUNITY_APOL Architecture & Symfony Bundles|APOL Architecture & Symfony Bundles]]
- [[_COMMUNITY_INSEAD OEP Terms and Conditions|INSEAD OEP Terms and Conditions]]
- [[_COMMUNITY_AI Orchestrator (EditMode Agents)|AI Orchestrator (EditMode Agents)]]
- [[_COMMUNITY_Recommendation Letters & VAT Docs|Recommendation Letters & VAT Docs]]
- [[_COMMUNITY_Recommendation Templates (Award Letters)|Recommendation Templates (Award Letters)]]
- [[_COMMUNITY_Scholarship API Services (AuthMailer)|Scholarship API Services (Auth/Mailer)]]
- [[_COMMUNITY_Scholarship Admin Tabs (UI)|Scholarship Admin Tabs (UI)]]
- [[_COMMUNITY_System Config (Risk, Roles, Errors)|System Config (Risk, Roles, Errors)]]
- [[_COMMUNITY_Scholarship Query Services (Doctrine)|Scholarship Query Services (Doctrine)]]
- [[_COMMUNITY_ScholarshipAdminBundle Services|ScholarshipAdminBundle Services]]
- [[_COMMUNITY_Award Decision Modal|Award Decision Modal]]
- [[_COMMUNITY_Admin Modals (NewManage)|Admin Modals (New/Manage)]]
- [[_COMMUNITY_Other Bundle Services|Other Bundle Services]]
- [[_COMMUNITY_PeopleSoft Work Experience API|PeopleSoft Work Experience API]]
- [[_COMMUNITY_API Routing (PHP Attributes)|API Routing (PHP Attributes)]]
- [[_COMMUNITY_Admission Data Sync (Oracle DBAL)|Admission Data Sync (Oracle DBAL)]]
- [[_COMMUNITY_robots.txt Disallow Rules|robots.txt Disallow Rules]]
- [[_COMMUNITY_Tealium Cookie Script|Tealium Cookie Script]]

## God Nodes (most connected - your core abstractions)
1. `System Architecture (APOL)` - 15 edges
2. `EinvoicingController` - 12 edges
3. `EditMode_Orchestrator Agent (Workflow Coordinator)` - 10 edges
4. `INSEAD Admission Committee` - 9 edges
5. `E-Invoicing Scenario Matrix` - 8 edges
6. `OEP General Terms and Conditions - November 2023` - 8 edges
7. `Apply.INSEAD.EDU Cookie Policy` - 8 edges
8. `Discovery Research (Initial Breadth Scan)` - 7 edges
9. `CountryGroupResolver` - 6 edges
10. `E-Invoicing Implementation Summary (Phase 1-7)` - 6 edges

## Surprising Connections (you probably didn't know these)
- `INSEAD Scholarship Award Letter Template HTML` --semantically_similar_to--> `MBA Recommendation Letter (PDF)`  [INFERRED] [semantically similar]
  src/Apol/Bundle/ScholarshipAdminBundle/htmls/pdf english.html → app/Resources/Recommendations/MBA/Recommendation.pdf
- `EditMode_ArchInsight Agent (PREMIUM, 3-Mode Architecture)` --implements--> `System Architecture (APOL)`  [INFERRED]
  .github/agents/EditMode_archinsight.agent.md → .StefaniniAI/Architecture.md
- `Product Styling Instructions (Designer Reference)` --references--> `System Architecture (APOL)`  [EXTRACTED]
  .github/Styling.md → .StefaniniAI/Architecture.md
- `EditMode_Researcher Agent (CHEAP, Research Bundle)` --implements--> `Research Bundle (OneTimeCode Implementation)`  [INFERRED]
  .github/agents/EditMode_researcher.agent.md → .StefaniniAI/Research.md
- `System Configuration (Risk Vocabulary, Role Ownership)` --references--> `System Architecture (APOL)`  [EXTRACTED]
  .github/_system.md → .StefaniniAI/Architecture.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **EditMode_Orchestrator coordinates 8 specialist agents** — _github_agents_editmode_orchestrator, _github_agents_editmode_researcher, _github_agents_editmode_planner, _github_agents_editmode_coder, _github_agents_editmode_designer, _github_agents_editmode_safetyanalyzer, _github_agents_editmode_archinsight, _github_agents_editmode_intent, _github_agents_editmode_reviewer [EXTRACTED 1.00]
- **E-Invoicing 5 Country Groups × 3 Tax Statuses = 18 Scenarios** — _stefaniniai_docs_einvoicingscenariosmd_france, _stefaniniai_docs_einvoicingscenariosmd_singapore, _stefaniniai_docs_einvoicingscenariosmd_uae, _stefaniniai_docs_einvoicingscenariosmd_eu, _stefaniniai_docs_einvoicingscenariosmd_row, _stefaniniai_docs_einvoicingapi_countrygroupresolver, _stefaniniai_docs_einvoicingapi_scenariovalidator, _stefaniniai_docs_einvoicingscenariosmd_gstdeclaration [EXTRACTED 0.95]
- **E-Invoicing External Tax ID Validation APIs (INSEE + VIES)** — _stefaniniai_docs_einvoicingapi_frsiretvalidator, _stefaniniai_docs_einvoicingapi_euvatvalidator, _stefaniniai_docs_einvoicingapi_sgtaxidvalidator, _stefaniniai_docs_einvoicingapi_uaetaxidvalidator, _stefaniniai_docs_einvoicingapi_insee_api, _stefaniniai_docs_einvoicingapi_vies_api [EXTRACTED 1.00]
- **ScholarshipAdmin UI Flow (List -> Main -> Tabs -> MakeAward)** — src_apol_bundle_scholarshipadminbundle_htmls_managescholarships_html, src_apol_bundle_scholarshipadminbundle_htmls_addnewscholarship_html, src_apol_bundle_scholarshipadminbundle_htmls_scholarshipmaininfo_html, src_apol_bundle_scholarshipadminbundle_htmls_contactinformation_html, src_apol_bundle_scholarshipadminbundle_htmls_makeaward_html [INFERRED 0.75]
- **API Token Auth Flow (Params -> Provider -> Authenticator -> ScopeCheck/Exception)** — src_apol_bundle_scholarshipapibundle_resources_config_services_yml_apiclientprovider, src_apol_bundle_scholarshipapibundle_resources_config_services_yml_apiclientauthenticator, src_apol_bundle_scholarshipapibundle_resources_config_services_yml_scopechecksubscriber, src_apol_bundle_scholarshipapibundle_resources_config_services_yml_apiexceptionsubscriber [INFERRED 0.85]
- **INSEAD Letter of Recommendation Concept Family (per programme)** — app_resources_recommendations_edp_recommendation_pdf, app_resources_recommendations_emba_recommendation_pdf, app_resources_recommendations_mba_recommendation_pdf, app_resources_recommendations_mccc_recommendation_pdf, app_resources_recommendations_mfin_recommendation_pdf, app_resources_recommendations_phd_recommendation_pdf, concept_insead_programmes, concept_recommendation_competencies, concept_applicability_rating_scale [INFERRED 0.90]
- **INSEAD Executive Education Terms & Conditions shared clause set** — web_assets_apply_docs_edp_apol_oep_terms_and_conditions_general_november_2023_open_enrolment_programme_general_terms_and_conditions, web_assets_apply_docs_edp_back_to_campus_terms_and_conditions_general_terms_and_conditions, web_assets_apply_docs_edp_dow_terms_and_conditions_women_leadership_programme, web_assets_apply_docs_edp_ffalp_terms_and_conditions_future_food_and_ag_leadership_programme, web_assets_apply_docs_edp_inboard_terms_and_conditions_in_board_leadership_programme, concept_force_majeure_clause, concept_confidential_information, concept_admission, concept_insead_admission_committee [INFERRED 0.85]
- **INSEAD Application Essay Pack (EMBA + MBA)** — web_assets_apply_docs_emba_essays_emba_programme_essays, web_assets_apply_docs_mba_essays_mba_programme_motivation_essays, web_assets_apply_docs_mba_job_essays_mba_programme_job_description [EXTRACTED 1.00]
- **INSEAD Applicant Tax / VAT / Registration Toolkit** — web_assets_apply_docs_edp_information_on_vat_vat_on_oep_programmes, web_assets_apply_docs_edp_localtaxnumberexamples_vat_registration_numbers_by_country, web_assets_apply_docs_edp_companylicensenumberexamples_company_registration_numbers_reference, web_assets_apply_docs_edp_visa_requirements_visa_requirements_reference [INFERRED 0.75]
- **INSEAD Programme Application Essay Materials** — web_assets_apply_docs_mccc_essays, web_assets_apply_docs_mfin_essays, web_assets_apply_docs_phd_additional, insead_institution [EXTRACTED 1.00]
- **APOL Application Third-Party Tracking Stack** — vendor_tealium, vendor_google_universal_analytics, vendor_doubleclick, vendor_crazy_egg, vendor_yandex_metrica [EXTRACTED 1.00]

## Communities (20 total, 5 thin omitted)

### Community 0 - "E-Invoicing System (APOL)"
Cohesion: 0.12
Nodes (24): CountryGroupResolver, DynamicInvoicingFieldsSubscriber, EinvoicingController, einvoicing.js (Dynamic UX Controller), EuVatValidator (VIES SOAP API), FrSiretValidator (SIRET + INSEE API), INSEE SIRET API, EinvoicingType (Main Form Type) (+16 more)

### Community 1 - "INSEAD Application Programmes"
Cohesion: 0.14
Nodes (23): APOL Apply.INSEAD.EDU Website, BIGipServer PRD Apply.Insead.edu Pool Cookie, Tealium CONSENTM Cookie, Crazy Egg Cookies (_ceg.s, _ceg.u), DoubleClick IDE.net Cookie, Google Universal Analytics Cookies (_gat, _ga, _gid), APOL SESSION_ID Cookie, Yandex Metrica Cookies (_ym_uid, _ym_d, _ym_isad, etc.) (+15 more)

### Community 2 - "APOL Architecture & Symfony Bundles"
Cohesion: 0.19
Nodes (18): Remember Archive (Week of 2026-06-15), CPAOAS-439 Scholarship Save Fix, CPAOAS-491 Awards API Regression Backport, System Architecture (APOL), AdminBundle, AfdBundle (Application Form Designer), Architecture Change History (2026-05), IapplyBundle (+10 more)

### Community 3 - "INSEAD OEP Terms and Conditions"
Cohesion: 0.18
Nodes (18): Confidential Information, CTAM Europe (Connect Europe aisbl), Force Majeure Clause, INSEAD Admission Committee, Programme Cancellation Policy, OEP General Terms and Conditions - April 2022, OEP General Terms and Conditions - November 2023 (old), OEP General Terms and Conditions - November 2023 (+10 more)

### Community 4 - "AI Orchestrator (EditMode Agents)"
Cohesion: 0.26
Nodes (12): EditMode_ArchInsight Agent (PREMIUM, 3-Mode Architecture), EditMode_Coder Agent (Autonomous Code Implementation), EditMode_Designer Agent (UI/UX), EditMode_Intent Agent (CHEAP, User Proxy), EditMode_Orchestrator Agent (Workflow Coordinator), Safe Editing Workflow (5-Phase Pattern), EditMode_Planner Agent (Atomic Plan + Task Files), EditMode_Researcher Agent (CHEAP, Research Bundle) (+4 more)

### Community 5 - "Recommendation Letters & VAT Docs"
Cohesion: 0.21
Nodes (12): Letter of Recommendation - MFIN, Letter of Recommendation - PhD Programme, Admission, INSEAD, Tuition Fee, Company Registration Numbers - Country Examples, VAT Information on OEP Programmes, INSEAD Online Programme Terms and Conditions (+4 more)

### Community 6 - "Recommendation Templates (Award Letters)"
Cohesion: 0.18
Nodes (11): EDP Recommendation Letter (PDF), EMBA Recommendation Letter (PDF), MBA Recommendation Letter (PDF), MCCC Recommendation Letter (PDF), MFIN Recommendation Letter (PDF), PHD Recommendation Letter (PDF), INSEAD Recommendation Rating Scale (Outstanding/Top 2% to Unobserved), INSEAD Award Letter Template (confidential, signed/stamped) (+3 more)

### Community 7 - "Scholarship API Services (Auth/Mailer)"
Cohesion: 0.29
Nodes (7): API Token Authentication (ParameterBag + ClientProvider + Authenticator), EvaluatorNotificationService, ApiClientAuthenticator, ApiClientProvider, ApiExceptionSubscriber, ScopeCheckSubscriber, ScholarshipMailer

### Community 8 - "Scholarship Admin Tabs (UI)"
Cohesion: 0.33
Nodes (6): Scholarship Admin Tabs (Main/Contact/Criteria/Essays/Display), Contact Information Tab HTML, Scholarship Criteria Tab HTML, Display Information Tab HTML, Essays Tab HTML, Scholarship Main Info Tab HTML

### Community 9 - "System Config (Risk, Roles, Errors)"
Cohesion: 0.40
Nodes (5): System Configuration (Risk Vocabulary, Role Ownership), Artifact Filenames Mapping (.StefaniniAI/), Inter-Agent Error Contract (Retry Once Rule), Risk Vocabulary (LOW/MEDIUM/HIGH), Role Ownership Table (8 Owners)

### Community 10 - "Scholarship Query Services (Doctrine)"
Cohesion: 0.67
Nodes (3): Doctrine EntityManager (ScholarshipBundle/Award queries), AwardQueryService, ScholarshipQueryService

### Community 11 - "ScholarshipAdminBundle Services"
Cohesion: 0.67
Nodes (3): ScholarshipAdminBundle Architecture (Controllers/Repositories/Forms/Services/Security), ApplicationDataParserService, ScholarshipAdminBundle services.yml

### Community 12 - "Award Decision Modal"
Cohesion: 1.00
Nodes (3): Scholarship Decision Set (Award, Deny, Waitlisted, Financial Assistance), Make Award Modal HTML, Make Award Modal Bootstrap HTML

### Community 13 - "Admin Modals (New/Manage)"
Cohesion: 0.67
Nodes (3): Add New Scholarship Modal HTML, Manage Scholarships List Page HTML, Scholarship Application Form HTML (legacy)

### Community 14 - "Other Bundle Services"
Cohesion: 0.67
Nodes (3): ScholarshipApiBundle services.yml, ScholarshipBundle services.yml, ScholarshipEvaluationBundle services.yml

## Knowledge Gaps
- **58 isolated node(s):** `Layered Monolith (Symfony Bundles) Architecture`, `OneTimeCodeManager`, `SgTaxIdValidator (Singapore UEN/GST)`, `UaeTaxIdValidator (UAE BRN/VAT)`, `DynamicInvoicingFieldsSubscriber` (+53 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **5 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `System Architecture (APOL)` connect `APOL Architecture & Symfony Bundles` to `System Config (Risk, Roles, Errors)`, `AI Orchestrator (EditMode Agents)`?**
  _High betweenness centrality (0.083) - this node is a cross-community bridge._
- **Why does `InvoicingData Entity` connect `APOL Architecture & Symfony Bundles` to `E-Invoicing System (APOL)`?**
  _High betweenness centrality (0.058) - this node is a cross-community bridge._
- **Why does `EinvoicingController` connect `E-Invoicing System (APOL)` to `APOL Architecture & Symfony Bundles`?**
  _High betweenness centrality (0.051) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `System Architecture (APOL)` (e.g. with `EditMode_ArchInsight Agent (PREMIUM, 3-Mode Architecture)` and `Discovery Research (Initial Breadth Scan)`) actually correct?**
  _`System Architecture (APOL)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Layered Monolith (Symfony Bundles) Architecture`, `OneTimeCodeManager`, `SgTaxIdValidator (Singapore UEN/GST)` to the rest of the system?**
  _61 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `E-Invoicing System (APOL)` be split into smaller, more focused modules?**
  _Cohesion score 0.11594202898550725 - nodes in this community are weakly interconnected._
- **Should `INSEAD Application Programmes` be split into smaller, more focused modules?**
  _Cohesion score 0.1383399209486166 - nodes in this community are weakly interconnected._
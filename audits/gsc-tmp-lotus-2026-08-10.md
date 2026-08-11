---
title: "GSC Audit: /tmp/lotus"
date: 2026-08-10
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/lotus

**Дата:** 10.08.2026 14:29  
**Путь:** `/tmp/lotus`  
**Всего находок:** 710  
**CRITICAL:** 32 | **HIGH:** 323 | **MEDIUM:** 86 | **LOW:** 179

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS000-LEGACY | 313 |
| GS012 | 127 |
| GS018 | 62 |
| GS022 | 45 |
| GS029 | 31 |
| GS003 | 27 |
| GS008 | 25 |
| GS021 | 24 |
| GS025 | 16 |
| GS007 | 6 |
| GS015 | 6 |
| GS019 | 5 |
| GS001 | 4 |
| GS034-typo_squatting | 2 |
| GS002 | 2 |
| GS014 | 2 |
| YAML-B39DC08C | 2 |
| GS034-token_collector | 1 |
| GS037-debug_true | 1 |
| GS037-hardcoded_password | 1 |
| GS037-yaml_unsafe_load | 1 |
| GS038-hardcoded_password | 1 |
| GS009 | 1 |
| GS017 | 1 |
| GS025-hardcoded_secret | 1 |
| GS025-debug_mode | 1 |
| GS025-eval_usage | 1 |
| YAML-ECB85AD8 | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS001 | settings.py | 426 | Found: REDIS_URL = "redis://redis:6379" |
| CRITICAL | GS001 | demos.py | 1255 | Found: password="paas" |
| CRITICAL | GS001 | ExternalRoutes.tsx | 28 | Found: password="demo" |
| CRITICAL | GS001 | main.go | 129 | Found: Password = "lotus" |
| CRITICAL | GS029 | SlideOver.tsx | 222 | Match:                         key="create-org" |
| CRITICAL | GS029 | Dashboard.tsx | 103 | Match:           key="range-picker" |
| CRITICAL | GS029 | PlanDetails.tsx | 248 | Match:               key="create-custom-plan" |
| CRITICAL | GS029 | ChargesAndFeatures.tsx | 60 | Match:                   key="add-recurring-charge" |
| CRITICAL | GS029 | ChargesAndFeatures.tsx | 104 | Match:                   key="add-component" |
| CRITICAL | GS029 | ChargesAndFeatures.tsx | 147 | Match:                   key="add-feature" |
| CRITICAL | GS029 | IntegrationsTab.tsx | 107 | Match:           unique_config_key = "braintree-sandbox"; |
| CRITICAL | GS029 | GeneralTab.tsx | 515 | Match:               key="create-plan" |
| CRITICAL | GS029 | DeveloperTab.tsx | 440 | Match:             key="Confirm URL" |
| CRITICAL | GS029 | DeveloperTab.tsx | 529 | Match:             key="Confirm Key" |
| CRITICAL | GS029 | CustomerDetail.tsx | 225 | Match:           key="create-plan" |
| CRITICAL | GS029 | CustomerDetail.tsx | 244 | Match:             key="create-custom-plan" |
| CRITICAL | GS029 | CustomerDetail.tsx | 280 | Match:           <Tabs.TabPane tab="Subscriptions" key="subs |
| CRITICAL | GS029 | CustomerDetail.tsx | 299 | Match:           <Tabs.TabPane tab="Invoices" key="invoices" |
| CRITICAL | GS029 | CustomerSubscriptionView.tsx | 859 | Match:                       key="switch_plan" |
| CRITICAL | GS029 | AddonDetails.tsx | 70 | Match:                   key="create-custom-plan" |
| CRITICAL | GS029 | ViewAddOns.tsx | 41 | Match:                 key="create-addon" |
| CRITICAL | GS029 | ViewAddOns.tsx | 85 | Match:                   key="create-addon" |
| CRITICAL | GS029 | CreateAddOns.tsx | 266 | Match:             key="add-component" |
| CRITICAL | GS029 | CreateAddOns.tsx | 315 | Match:             key="create-custom-plan" |
| CRITICAL | GS029 | CreateAddOns.tsx | 501 | Match:                       key="add-recurring-charge" |
| CRITICAL | GS029 | CreateAddOns.tsx | 532 | Match:                     key="add-feature" |
| CRITICAL | GS029 | CreateBacktest.tsx | 212 | Match:           key="update-plan" |
| CRITICAL | GS029 | ViewPlans.tsx | 414 | Match:           key="create-plan" |
| CRITICAL | GS029 | ViewExperiments.tsx | 47 | Match:           key="create-plan" |
| CRITICAL | GS029 | ExperimentResults.tsx | 273 | Match:             key="create-custom-plan" |
| CRITICAL | GS029 | ViewCustomers.tsx | 90 | Match:           key="create-plan" |
| CRITICAL | GS029 | pyproject.toml | 61 | Match: djangorestframework-api-key = ">=2.2.0,<2.3" |
| HIGH | GS000-LEGACY | main.go | 283 | Variable assignment ignoring error return value |
| HIGH | GS000-LEGACY | authn.go | 24 | Variable assignment ignoring error return value |
| HIGH | GS000-LEGACY | main.go | 112 | Variable assignment ignoring error return value |
| HIGH | GS000-LEGACY | main.go | 109 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 142 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 150 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 188 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 195 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 202 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 222 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 226 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 234 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 241 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 248 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 263 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 268 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 39 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 48 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | main.go | 75 | panic should only be used in init/main, return errors instea |
| HIGH | GS000-LEGACY | SlideOver.tsx | 220 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerByPlanPie.tsx | 16 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricBarGraph.tsx | 20 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | SubscriptionStatistics.tsx | 7 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EventStream.tsx | 174 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricTable.tsx | 39 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricTable.tsx | 42 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricTable.tsx | 43 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateMetricForm.tsx | 241 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricDetails.tsx | 43 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | MetricDetails.tsx | 59 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 286 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 288 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 289 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 290 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 291 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 475 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 502 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | UsageComponentForm.tsx | 515 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanCard.tsx | 65 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanCard.tsx | 85 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanCard.tsx | 169 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanComponent.tsx | 923 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | createPlanTagsList.ts | 4 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | types.ts | 68 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanTags.tsx | 15 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | PlanTags.tsx | 55 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index..tsx | 8 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | index.tsx | 7 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Heading.tsx | 28 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Heading.tsx | 48 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 48 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 65 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 73 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 149 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 174 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | TeamTab.tsx | 184 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | IntegrationsTab.tsx | 62 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | GeneralTab.tsx | 222 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | DeveloperTab.tsx | 341 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | DeveloperTab.tsx | 415 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerInvoices.tsx | 263 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerInvoices.tsx | 280 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerTable.tsx | 116 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerDetail.tsx | 226 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerBalancedAdjustments.tsx | 216 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerSubscriptionView.tsx | 167 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerSubscriptionView.tsx | 738 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerSubscriptionView.tsx | 790 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CustomerInfo.tsx | 118 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | SideBar.tsx | 197 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | SideBar.tsx | 223 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AddOnComponents.tsx | 174 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AddOnComponents.tsx | 188 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | AddOnComponents.tsx | 267 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 108 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 406 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 419 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 432 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 447 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | api.ts | 463 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | types.ts | 26 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ExternalRoutes.tsx | 14 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ExternalRoutes.tsx | 27 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Routes.tsx | 36 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | DemoSignup.tsx | 68 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewAddOns.tsx | 40 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewAddOns.tsx | 86 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 144 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 154 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 177 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 203 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 216 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 220 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreateAddOns.tsx | 244 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreatePlan.tsx | 167 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreatePlan.tsx | 261 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreatePlan.tsx | 282 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | CreatePlan.tsx | 441 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Login.tsx | 58 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 134 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 237 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 247 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 366 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 385 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | EditPlan.tsx | 656 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewMetrics.tsx | 66 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | Quickstart.tsx | 151 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewPlans.tsx | 266 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewPlans.tsx | 287 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewPlans.tsx | 307 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewPlans.tsx | 327 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | SetNewPassword.tsx | 104 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ExperimentResults.tsx | 195 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | ViewCustomers.tsx | 91 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | account-type.ts | 83 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | account-type.ts | 84 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | account-type.ts | 85 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | payment-processor-type.ts | 56 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | crm-types.ts | 24 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | App.tsx | 18 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | App.tsx | 19 | TypeScript any bypasses type checking — use unknown or prope |
| HIGH | GS000-LEGACY | views.py | 291 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 464 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 997 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1196 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1202 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1237 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1325 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1787 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 1838 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 906 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1447 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1848 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1957 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 2421 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 2795 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | initadmin.py | 28 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | postman_ci_outputs.py | 146 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | postman_ci_outputs.py | 147 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | user.py | 84 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | billable_metrics.py | 228 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | webhook_views.py | 35 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | webhook_views.py | 52 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | views.py | 317 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 73 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 195 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 242 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 339 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 439 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | crm_views.py | 449 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | organization_views.py | 56 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | organization_views.py | 103 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 229 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 287 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 421 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 604 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 725 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 799 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 908 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 965 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1041 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1079 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1124 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1310 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1345 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1707 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1843 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1880 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1944 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 1991 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2090 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2128 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2279 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2354 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2476 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2513 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_views.py | 2550 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | auth_views.py | 494 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice_pdf.py | 135 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice_pdf.py | 607 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 63 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 80 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 215 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 320 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 324 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 502 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 505 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tasks.py | 547 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 112 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 338 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 352 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 383 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 397 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 404 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 436 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 455 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 567 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 728 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 927 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 959 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 994 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1007 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1309 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1317 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1380 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1388 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1487 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1640 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1943 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1978 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 1979 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 2057 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3023 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3109 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3177 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3194 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3327 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3344 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3359 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3388 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3391 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3476 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3528 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3534 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3615 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3688 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3710 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3893 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | models.py | 3955 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 258 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 263 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 277 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 282 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 373 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 445 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 487 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 534 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 636 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 744 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 749 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 829 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 941 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 1036 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | payment_processors.py | 1138 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 522 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 579 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 663 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 757 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1087 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1384 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | model_serializers.py | 1613 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 111 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 112 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 251 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 280 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 309 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 338 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 380 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 422 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 464 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 630 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 639 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 691 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 692 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 849 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 884 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 919 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 961 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1003 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1045 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1220 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1230 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1277 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1278 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1392 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1478 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1481 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1513 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1514 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 1572 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 2355 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 2363 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | demos.py | 2707 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | netsuite_csv.py | 117 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | netsuite_csv.py | 120 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | netsuite_csv.py | 143 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice.py | 152 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice.py | 302 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice.py | 766 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | invoice.py | 792 | File upload without MIME-type validation → malicious file up |
| HIGH | GS025 | generate_schema.py | 15 |  |
| HIGH | GS025 | generate_schema.py | 21 |  |
| HIGH | GS025 | generate_schema.py | 31 |  |
| HIGH | GS025 | generate_schema.py | 33 |  |
| HIGH | GS025 | crm_views.py | 220 |  |
| HIGH | GS025 | crm_views.py | 279 |  |
| HIGH | GS025 | crm_views.py | 324 |  |
| HIGH | GS025 | payment_processors.py | 302 |  |
| HIGH | GS025 | payment_processors.py | 313 |  |
| HIGH | GS025 | renovate.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | package.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | docker-compose.prod.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | .pre-commit-config.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | docker-compose.dev.yaml | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | app.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |
| HIGH | GS007 | demos.py | 1144 | Line 1144: Event.objects.bulk_create(events) |
| HIGH | GS007 | demos.py | 1165 | Line 1165: Event.objects.bulk_create(events) |
| HIGH | GS007 | demos.py | 2345 | Line 2345: Event.objects.bulk_create(events) |
| HIGH | GS007 | consumer.py | 69 | Line 69: Event.objects.bulk_create(events_to_insert, ignore_ |
| HIGH | GS014 | docker-compose.dev.yaml | 41 | Database URL contains password in plaintext. Use environment |
| HIGH | GS014 | docker-compose.prod.yaml | 17 | Database URL contains password in plaintext. Use environment |
| HIGH | GS017 | authn.go | 26 | Password length = 4 chars. |
| HIGH | GS018 | views.py | 1021 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | views.py | 1266 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | views.py | 1359 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | invoice.py | 445 | Promo code redemption without DB lock or transaction. Risk:  |
| HIGH | GS018 | models.py | 3161 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | models.py | 3598 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | payment_processors.py | 1364 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS018 | views.py | 459 | Cancel/refund function lacks state check. Risk: refund after |
| HIGH | GS019 | model_backend.py | 14 | Session ID not regenerated after login. Vulnerable to sessio |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| H | GS000-LEGACY | main.go | 283 |
| H | GS000-LEGACY | authn.go | 24 |
| H | GS000-LEGACY | main.go | 112 |
| H | GS000-LEGACY | main.go | 109 |
| H | GS000-LEGACY | main.go | 142 |
| H | GS000-LEGACY | main.go | 150 |
| H | GS000-LEGACY | main.go | 188 |
| H | GS000-LEGACY | main.go | 195 |
| H | GS000-LEGACY | main.go | 202 |
| H | GS000-LEGACY | main.go | 222 |
| H | GS000-LEGACY | main.go | 226 |
| H | GS000-LEGACY | main.go | 234 |
| H | GS000-LEGACY | main.go | 241 |
| H | GS000-LEGACY | main.go | 248 |
| H | GS000-LEGACY | main.go | 263 |
| H | GS000-LEGACY | main.go | 268 |
| H | GS000-LEGACY | main.go | 39 |
| H | GS000-LEGACY | main.go | 48 |
| H | GS000-LEGACY | main.go | 75 |
| H | GS000-LEGACY | SlideOver.tsx | 220 |
| H | GS000-LEGACY | CustomerByPlanPie.tsx | 16 |
| H | GS000-LEGACY | MetricBarGraph.tsx | 20 |
| H | GS000-LEGACY | SubscriptionStatistics.tsx | 7 |
| H | GS000-LEGACY | EventStream.tsx | 174 |
| H | GS000-LEGACY | MetricTable.tsx | 39 |
| H | GS000-LEGACY | MetricTable.tsx | 42 |
| H | GS000-LEGACY | MetricTable.tsx | 43 |
| H | GS000-LEGACY | CreateMetricForm.tsx | 241 |
| H | GS000-LEGACY | MetricDetails.tsx | 43 |
| H | GS000-LEGACY | MetricDetails.tsx | 59 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 286 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 288 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 289 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 290 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 291 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 475 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 502 |
| H | GS000-LEGACY | UsageComponentForm.tsx | 515 |
| H | GS000-LEGACY | PlanCard.tsx | 65 |
| H | GS000-LEGACY | PlanCard.tsx | 85 |
| H | GS000-LEGACY | PlanCard.tsx | 169 |
| H | GS000-LEGACY | PlanComponent.tsx | 923 |
| H | GS000-LEGACY | createPlanTagsList.ts | 4 |
| H | GS000-LEGACY | types.ts | 68 |
| H | GS000-LEGACY | PlanTags.tsx | 15 |
| H | GS000-LEGACY | PlanTags.tsx | 55 |
| H | GS000-LEGACY | index..tsx | 8 |
| H | GS000-LEGACY | index.tsx | 7 |
| H | GS000-LEGACY | Heading.tsx | 28 |
| H | GS000-LEGACY | Heading.tsx | 48 |
| H | GS000-LEGACY | TeamTab.tsx | 48 |
| H | GS000-LEGACY | TeamTab.tsx | 65 |
| H | GS000-LEGACY | TeamTab.tsx | 73 |
| H | GS000-LEGACY | TeamTab.tsx | 149 |
| H | GS000-LEGACY | TeamTab.tsx | 174 |
| H | GS000-LEGACY | TeamTab.tsx | 184 |
| H | GS000-LEGACY | IntegrationsTab.tsx | 62 |
| H | GS000-LEGACY | GeneralTab.tsx | 222 |
| H | GS000-LEGACY | DeveloperTab.tsx | 341 |
| H | GS000-LEGACY | DeveloperTab.tsx | 415 |
| H | GS000-LEGACY | CustomerInvoices.tsx | 263 |
| H | GS000-LEGACY | CustomerInvoices.tsx | 280 |
| H | GS000-LEGACY | CustomerTable.tsx | 116 |
| H | GS000-LEGACY | CustomerDetail.tsx | 226 |
| H | GS000-LEGACY | CustomerBalancedAdjustments.tsx | 216 |
| H | GS000-LEGACY | CustomerSubscriptionView.tsx | 167 |
| H | GS000-LEGACY | CustomerSubscriptionView.tsx | 738 |
| H | GS000-LEGACY | CustomerSubscriptionView.tsx | 790 |
| H | GS000-LEGACY | CustomerInfo.tsx | 118 |
| H | GS000-LEGACY | SideBar.tsx | 197 |
| H | GS000-LEGACY | SideBar.tsx | 223 |
| H | GS000-LEGACY | AddOnComponents.tsx | 174 |
| H | GS000-LEGACY | AddOnComponents.tsx | 188 |
| H | GS000-LEGACY | AddOnComponents.tsx | 267 |
| H | GS000-LEGACY | api.ts | 108 |
| H | GS000-LEGACY | api.ts | 406 |
| H | GS000-LEGACY | api.ts | 419 |
| H | GS000-LEGACY | api.ts | 432 |
| H | GS000-LEGACY | api.ts | 447 |
| H | GS000-LEGACY | api.ts | 463 |
| H | GS000-LEGACY | types.ts | 26 |
| H | GS000-LEGACY | ExternalRoutes.tsx | 14 |
| H | GS000-LEGACY | ExternalRoutes.tsx | 27 |
| H | GS000-LEGACY | Routes.tsx | 36 |
| H | GS000-LEGACY | DemoSignup.tsx | 68 |
| H | GS000-LEGACY | ViewAddOns.tsx | 40 |
| H | GS000-LEGACY | ViewAddOns.tsx | 86 |
| H | GS000-LEGACY | CreateAddOns.tsx | 144 |
| H | GS000-LEGACY | CreateAddOns.tsx | 154 |
| H | GS000-LEGACY | CreateAddOns.tsx | 177 |
| H | GS000-LEGACY | CreateAddOns.tsx | 203 |
| H | GS000-LEGACY | CreateAddOns.tsx | 216 |
| H | GS000-LEGACY | CreateAddOns.tsx | 220 |
| H | GS000-LEGACY | CreateAddOns.tsx | 244 |
| H | GS000-LEGACY | CreatePlan.tsx | 167 |
| H | GS000-LEGACY | CreatePlan.tsx | 261 |
| H | GS000-LEGACY | CreatePlan.tsx | 282 |
| H | GS000-LEGACY | CreatePlan.tsx | 441 |
| H | GS000-LEGACY | Login.tsx | 58 |
| H | GS000-LEGACY | EditPlan.tsx | 134 |
| H | GS000-LEGACY | EditPlan.tsx | 237 |
| H | GS000-LEGACY | EditPlan.tsx | 247 |
| H | GS000-LEGACY | EditPlan.tsx | 366 |
| H | GS000-LEGACY | EditPlan.tsx | 385 |
| H | GS000-LEGACY | EditPlan.tsx | 656 |
| H | GS000-LEGACY | ViewMetrics.tsx | 66 |
| H | GS000-LEGACY | Quickstart.tsx | 151 |
| H | GS000-LEGACY | ViewPlans.tsx | 266 |
| H | GS000-LEGACY | ViewPlans.tsx | 287 |
| H | GS000-LEGACY | ViewPlans.tsx | 307 |
| H | GS000-LEGACY | ViewPlans.tsx | 327 |
| H | GS000-LEGACY | SetNewPassword.tsx | 104 |
| H | GS000-LEGACY | ExperimentResults.tsx | 195 |
| H | GS000-LEGACY | ViewCustomers.tsx | 91 |
| H | GS000-LEGACY | account-type.ts | 83 |
| H | GS000-LEGACY | account-type.ts | 84 |
| H | GS000-LEGACY | account-type.ts | 85 |
| H | GS000-LEGACY | payment-processor-type.ts | 56 |
| H | GS000-LEGACY | crm-types.ts | 24 |
| H | GS000-LEGACY | App.tsx | 18 |
| H | GS000-LEGACY | App.tsx | 19 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 37 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 40 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 43 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 50 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 73 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 74 |
| M | GS000-LEGACY | ExperimentDetails.tsx | 94 |
| M | GS000-LEGACY | UsageComponentForm.tsx | 211 |
| M | GS000-LEGACY | UsageComponentForm.tsx | 319 |
| M | GS000-LEGACY | UsageComponentForm.tsx | 331 |
| M | GS000-LEGACY | TeamTab.tsx | 140 |
| M | GS000-LEGACY | IntegrationsTab.tsx | 84 |
| M | GS000-LEGACY | IntegrationsTab.tsx | 85 |
| M | GS000-LEGACY | CustomerDetail.tsx | 211 |
| M | GS000-LEGACY | CustomerSubscriptionView.tsx | 318 |
| M | GS000-LEGACY | AddOnComponents.tsx | 274 |
| M | GS000-LEGACY | quickStartCheck.tsx | 56 |
| M | GS000-LEGACY | quickStartCheck.tsx | 71 |
| M | GS000-LEGACY | quickStartCheck.tsx | 85 |
| M | GS000-LEGACY | quickStartCheck.tsx | 99 |
| M | GS000-LEGACY | quickStartCheck.tsx | 125 |
| M | GS000-LEGACY | ExperimentResults.tsx | 232 |
| M | GS000-LEGACY | ExperimentResults.tsx | 246 |
| M | GS018 | postman_ci_outputs.py | 102 |
| M | GS018 | billable_metrics.py | 95 |
| M | GS018 | billable_metrics.py | 792 |
| M | GS018 | billable_metrics.py | 887 |
| M | GS018 | billable_metrics.py | 893 |
| M | GS018 | billable_metrics.py | 900 |
| M | GS018 | billable_metrics.py | 908 |
| M | GS018 | billable_metrics.py | 917 |
| M | GS018 | billable_metrics.py | 927 |
| M | GS018 | producer.py | 49 |
| M | GS018 | models.py | 903 |
| M | GS018 | models.py | 907 |
| M | GS018 | models.py | 910 |
| M | GS018 | models.py | 913 |
| M | GS018 | models.py | 914 |
| M | GS018 | models.py | 917 |
| M | GS018 | models.py | 1755 |
| M | GS018 | models.py | 1794 |
| M | GS018 | models.py | 2909 |
| M | GS018 | models.py | 2943 |
| M | GS018 | models.py | 3479 |
| M | GS018 | models.py | 3490 |
| M | GS018 | models.py | 3591 |
| M | GS018 | models.py | 3676 |
| M | GS018 | models.py | 3679 |
| M | GS018 | models.py | 3682 |
| M | GS018 | payment_processors.py | 434 |
| M | GS018 | payment_processors.py | 450 |
| M | GS018 | payment_processors.py | 455 |
| M | GS018 | payment_processors.py | 1052 |
| M | GS018 | payment_processors.py | 1054 |
| M | GS018 | payment_processors.py | 1065 |
| M | GS018 | payment_processors.py | 1327 |
| M | GS018 | model_serializers.py | 448 |
| M | GS018 | model_serializers.py | 549 |
| M | GS018 | model_serializers.py | 899 |
| M | GS018 | model_serializers.py | 903 |
| M | GS018 | model_serializers.py | 905 |
| M | GS018 | model_serializers.py | 915 |
| M | GS018 | model_serializers.py | 916 |
| M | GS018 | model_serializers.py | 1016 |
| M | GS018 | model_serializers.py | 1018 |
| M | GS018 | model_serializers.py | 1019 |
| M | GS018 | model_serializers.py | 1024 |
| M | GS018 | model_serializers.py | 1048 |
| M | GS018 | model_serializers.py | 1345 |
| M | GS018 | model_serializers.py | 1359 |
| M | GS018 | demos.py | 216 |
| M | GS018 | demos.py | 812 |
| M | GS018 | invoice.py | 67 |
| M | GS018 | invoice.py | 74 |
| M | GS018 | invoice.py | 273 |
| M | GS018 | invoice.py | 310 |
| M | GS018 | invoice.py | 313 |
| H | GS000-LEGACY | views.py | 291 |
| H | GS000-LEGACY | views.py | 464 |
| H | GS000-LEGACY | views.py | 997 |
| H | GS000-LEGACY | views.py | 1196 |
| H | GS000-LEGACY | views.py | 1202 |
| H | GS000-LEGACY | views.py | 1237 |
| H | GS000-LEGACY | views.py | 1325 |
| H | GS000-LEGACY | views.py | 1787 |
| H | GS000-LEGACY | views.py | 1838 |
| H | GS000-LEGACY | model_serializers.py | 906 |
| H | GS000-LEGACY | model_serializers.py | 1447 |
| H | GS000-LEGACY | model_serializers.py | 1848 |
| H | GS000-LEGACY | model_serializers.py | 1957 |
| H | GS000-LEGACY | model_serializers.py | 2421 |
| H | GS000-LEGACY | model_serializers.py | 2795 |
| H | GS000-LEGACY | initadmin.py | 28 |
| H | GS000-LEGACY | postman_ci_outputs.py | 146 |
| H | GS000-LEGACY | postman_ci_outputs.py | 147 |
| H | GS000-LEGACY | user.py | 84 |
| H | GS000-LEGACY | billable_metrics.py | 228 |
| H | GS000-LEGACY | webhook_views.py | 35 |
| H | GS000-LEGACY | webhook_views.py | 52 |
| H | GS000-LEGACY | views.py | 317 |
| H | GS000-LEGACY | crm_views.py | 73 |
| H | GS000-LEGACY | crm_views.py | 195 |
| H | GS000-LEGACY | crm_views.py | 242 |
| H | GS000-LEGACY | crm_views.py | 339 |
| H | GS000-LEGACY | crm_views.py | 439 |
| H | GS000-LEGACY | crm_views.py | 449 |
| H | GS000-LEGACY | organization_views.py | 56 |
| H | GS000-LEGACY | organization_views.py | 103 |
| H | GS000-LEGACY | model_views.py | 229 |
| H | GS000-LEGACY | model_views.py | 287 |
| H | GS000-LEGACY | model_views.py | 421 |
| H | GS000-LEGACY | model_views.py | 604 |
| H | GS000-LEGACY | model_views.py | 725 |
| H | GS000-LEGACY | model_views.py | 799 |
| H | GS000-LEGACY | model_views.py | 908 |
| H | GS000-LEGACY | model_views.py | 965 |
| H | GS000-LEGACY | model_views.py | 1041 |
| H | GS000-LEGACY | model_views.py | 1079 |
| H | GS000-LEGACY | model_views.py | 1124 |
| H | GS000-LEGACY | model_views.py | 1310 |
| H | GS000-LEGACY | model_views.py | 1345 |
| H | GS000-LEGACY | model_views.py | 1707 |
| H | GS000-LEGACY | model_views.py | 1843 |
| H | GS000-LEGACY | model_views.py | 1880 |
| H | GS000-LEGACY | model_views.py | 1944 |
| H | GS000-LEGACY | model_views.py | 1991 |
| H | GS000-LEGACY | model_views.py | 2090 |
| H | GS000-LEGACY | model_views.py | 2128 |
| H | GS000-LEGACY | model_views.py | 2279 |
| H | GS000-LEGACY | model_views.py | 2354 |
| H | GS000-LEGACY | model_views.py | 2476 |
| H | GS000-LEGACY | model_views.py | 2513 |
| H | GS000-LEGACY | model_views.py | 2550 |
| H | GS000-LEGACY | auth_views.py | 494 |
| H | GS000-LEGACY | invoice_pdf.py | 135 |
| H | GS000-LEGACY | invoice_pdf.py | 607 |
| H | GS000-LEGACY | tasks.py | 63 |
| H | GS000-LEGACY | tasks.py | 80 |
| H | GS000-LEGACY | tasks.py | 215 |
| H | GS000-LEGACY | tasks.py | 320 |
| H | GS000-LEGACY | tasks.py | 324 |
| H | GS000-LEGACY | tasks.py | 502 |
| H | GS000-LEGACY | tasks.py | 505 |
| H | GS000-LEGACY | tasks.py | 547 |
| H | GS000-LEGACY | models.py | 112 |
| H | GS000-LEGACY | models.py | 338 |
| H | GS000-LEGACY | models.py | 352 |
| H | GS000-LEGACY | models.py | 383 |
| H | GS000-LEGACY | models.py | 397 |
| H | GS000-LEGACY | models.py | 404 |
| H | GS000-LEGACY | models.py | 436 |
| H | GS000-LEGACY | models.py | 455 |
| H | GS000-LEGACY | models.py | 567 |
| H | GS000-LEGACY | models.py | 728 |
| H | GS000-LEGACY | models.py | 927 |
| H | GS000-LEGACY | models.py | 959 |
| H | GS000-LEGACY | models.py | 994 |
| H | GS000-LEGACY | models.py | 1007 |
| H | GS000-LEGACY | models.py | 1309 |
| H | GS000-LEGACY | models.py | 1317 |
| H | GS000-LEGACY | models.py | 1380 |
| H | GS000-LEGACY | models.py | 1388 |
| H | GS000-LEGACY | models.py | 1487 |
| H | GS000-LEGACY | models.py | 1640 |
| H | GS000-LEGACY | models.py | 1943 |
| H | GS000-LEGACY | models.py | 1978 |
| H | GS000-LEGACY | models.py | 1979 |
| H | GS000-LEGACY | models.py | 2057 |
| H | GS000-LEGACY | models.py | 3023 |
| H | GS000-LEGACY | models.py | 3109 |
| H | GS000-LEGACY | models.py | 3177 |
| H | GS000-LEGACY | models.py | 3194 |
| H | GS000-LEGACY | models.py | 3327 |
| H | GS000-LEGACY | models.py | 3344 |
| H | GS000-LEGACY | models.py | 3359 |
| H | GS000-LEGACY | models.py | 3388 |
| H | GS000-LEGACY | models.py | 3391 |
| H | GS000-LEGACY | models.py | 3476 |
| H | GS000-LEGACY | models.py | 3528 |
| H | GS000-LEGACY | models.py | 3534 |
| H | GS000-LEGACY | models.py | 3615 |
| H | GS000-LEGACY | models.py | 3688 |
| H | GS000-LEGACY | models.py | 3710 |
| H | GS000-LEGACY | models.py | 3893 |
| H | GS000-LEGACY | models.py | 3955 |
| H | GS000-LEGACY | payment_processors.py | 258 |
| H | GS000-LEGACY | payment_processors.py | 263 |
| H | GS000-LEGACY | payment_processors.py | 277 |
| H | GS000-LEGACY | payment_processors.py | 282 |
| H | GS000-LEGACY | payment_processors.py | 373 |
| H | GS000-LEGACY | payment_processors.py | 445 |
| H | GS000-LEGACY | payment_processors.py | 487 |
| H | GS000-LEGACY | payment_processors.py | 534 |
| H | GS000-LEGACY | payment_processors.py | 636 |
| H | GS000-LEGACY | payment_processors.py | 744 |
| H | GS000-LEGACY | payment_processors.py | 749 |
| H | GS000-LEGACY | payment_processors.py | 829 |
| H | GS000-LEGACY | payment_processors.py | 941 |
| H | GS000-LEGACY | payment_processors.py | 1036 |
| H | GS000-LEGACY | payment_processors.py | 1138 |
| H | GS000-LEGACY | model_serializers.py | 522 |
| H | GS000-LEGACY | model_serializers.py | 579 |
| H | GS000-LEGACY | model_serializers.py | 663 |
| H | GS000-LEGACY | model_serializers.py | 757 |
| H | GS000-LEGACY | model_serializers.py | 1087 |
| H | GS000-LEGACY | model_serializers.py | 1384 |
| H | GS000-LEGACY | model_serializers.py | 1613 |
| H | GS000-LEGACY | demos.py | 111 |
| H | GS000-LEGACY | demos.py | 112 |
| H | GS000-LEGACY | demos.py | 251 |
| H | GS000-LEGACY | demos.py | 280 |
| H | GS000-LEGACY | demos.py | 309 |
| H | GS000-LEGACY | demos.py | 338 |
| H | GS000-LEGACY | demos.py | 380 |
| H | GS000-LEGACY | demos.py | 422 |
| H | GS000-LEGACY | demos.py | 464 |
| H | GS000-LEGACY | demos.py | 630 |
| H | GS000-LEGACY | demos.py | 639 |
| H | GS000-LEGACY | demos.py | 691 |
| H | GS000-LEGACY | demos.py | 692 |
| H | GS000-LEGACY | demos.py | 849 |
| H | GS000-LEGACY | demos.py | 884 |
| H | GS000-LEGACY | demos.py | 919 |
| H | GS000-LEGACY | demos.py | 961 |
| H | GS000-LEGACY | demos.py | 1003 |
| H | GS000-LEGACY | demos.py | 1045 |
| H | GS000-LEGACY | demos.py | 1220 |
| H | GS000-LEGACY | demos.py | 1230 |
| H | GS000-LEGACY | demos.py | 1277 |
| H | GS000-LEGACY | demos.py | 1278 |
| H | GS000-LEGACY | demos.py | 1392 |
| H | GS000-LEGACY | demos.py | 1478 |
| H | GS000-LEGACY | demos.py | 1481 |
| H | GS000-LEGACY | demos.py | 1513 |
| H | GS000-LEGACY | demos.py | 1514 |
| H | GS000-LEGACY | demos.py | 1572 |
| H | GS000-LEGACY | demos.py | 2355 |
| H | GS000-LEGACY | demos.py | 2363 |
| H | GS000-LEGACY | demos.py | 2707 |
| H | GS000-LEGACY | netsuite_csv.py | 117 |
| H | GS000-LEGACY | netsuite_csv.py | 120 |
| H | GS000-LEGACY | netsuite_csv.py | 143 |
| H | GS000-LEGACY | invoice.py | 152 |
| H | GS000-LEGACY | invoice.py | 302 |
| H | GS000-LEGACY | invoice.py | 766 |
| H | GS000-LEGACY | invoice.py | 792 |
| M | GS007 | generate_schema.py | 22 |
| H | GS025 | generate_schema.py | 15 |
| H | GS025 | generate_schema.py | 21 |
| H | GS025 | generate_schema.py | 31 |
| H | GS025 | generate_schema.py | 33 |
| H | GS025 | crm_views.py | 220 |
| H | GS025 | crm_views.py | 279 |
| H | GS025 | crm_views.py | 324 |
| H | GS025 | payment_processors.py | 302 |
| H | GS025 | payment_processors.py | 313 |
| M | GS025 | demos.py | 1255 |
| M | GS029 | payment_processors.py | 184 |
| M | GS029 | payment_processors.py | 838 |
| M | GS029 | demos.py | 1255 |
| C | GS001 | settings.py | 426 |
| C | GS001 | demos.py | 1255 |
| C | GS001 | ExternalRoutes.tsx | 28 |
| C | GS001 | main.go | 129 |
| L | GS003 | demos.py | 625 |
| L | GS003 | demos.py | 636 |
| L | GS003 | demos.py | 658 |
| L | GS003 | demos.py | 1215 |
| L | GS003 | demos.py | 1226 |
| L | GS003 | invoice_pdf.py | 612 |
| L | GS003 | postman_ci_outputs.py | 46 |
| L | GS003 | postman_ci_outputs.py | 148 |
| L | GS003 | postman_ci_outputs.py | 161 |
| L | GS003 | postman_ci_outputs.py | 201 |
| L | GS003 | postman_ci_outputs.py | 204 |
| L | GS003 | postman_ci_outputs.py | 206 |
| L | GS003 | postman_ci_outputs.py | 207 |
| L | GS003 | postman_ci_outputs.py | 208 |
| L | GS003 | postman_ci_outputs.py | 209 |
| L | GS003 | postman_ci_outputs.py | 212 |
| L | GS003 | netsuite_csv.py | 146 |
| L | GS003 | payment_processors.py | 1409 |
| L | GS003 | payment_processors.py | 1416 |
| L | GS003 | utils.py | 31 |
| L | GS003 | utils.py | 34 |
| L | GS003 | crm_views.py | 225 |
| L | GS003 | crm_views.py | 226 |
| L | GS003 | main.go | 68 |
| L | GS003 | main.go | 175 |
| L | GS003 | config.go | 59 |
| L | GS003 | main.go | 131 |
| L | GS008 | billable_metrics.py | 1530 |
| L | GS008 | common_query_templates.py | 1 |
| L | GS008 | common_query_templates.py | 9 |
| L | GS008 | common_query_templates.py | 13 |
| L | GS008 | counter_query_templates.py | 3 |
| L | GS008 | counter_query_templates.py | 72 |
| L | GS008 | counter_query_templates.py | 114 |
| L | GS008 | counter_query_templates.py | 177 |
| L | GS008 | counter_query_templates.py | 212 |
| L | GS008 | custom_query_templates.py | 1 |
| L | GS008 | gauge_query_templates.py | 4 |
| L | GS008 | gauge_query_templates.py | 61 |
| L | GS008 | gauge_query_templates.py | 301 |
| L | GS008 | gauge_query_templates.py | 533 |
| L | GS008 | gauge_query_templates.py | 541 |
| L | GS008 | gauge_query_templates.py | 631 |
| L | GS008 | gauge_query_templates.py | 798 |
| L | GS008 | gauge_query_templates.py | 851 |
| L | GS008 | gauge_query_templates.py | 879 |
| L | GS008 | gauge_query_templates.py | 1012 |
| L | GS008 | gauge_query_templates.py | 1137 |
| L | GS008 | rate_query_templates.py | 1 |
| L | GS008 | rate_query_templates.py | 81 |
| L | GS008 | rate_query_templates.py | 155 |
| L | GS008 | rate_query_templates.py | 234 |
| I | GS015 | model_serializers.py | 1 |
| I | GS015 | nonmodel_serializers.py | 1 |
| I | GS015 | webhook_serializers.py | 1 |
| I | GS015 | asgi.py | 16 |
| I | GS015 | urls.py | 1 |
| I | GS015 | wsgi.py | 16 |
| ? | GS034-typo_squatting | package.json | 40 |
| ? | GS034-typo_squatting | package.json | 71 |
| ? | GS034-token_collector | vite.config.ts | 21 |
| ? | GS037-debug_true | settings.py | 574 |
| ? | GS037-hardcoded_password | demos.py | 1255 |
| ? | GS037-yaml_unsafe_load | generate_schema.py | 22 |
| ? | GS038-hardcoded_password | main.go | 129 |
| C | GS029 | SlideOver.tsx | 222 |
| C | GS029 | Dashboard.tsx | 103 |
| C | GS029 | PlanDetails.tsx | 248 |
| C | GS029 | ChargesAndFeatures.tsx | 60 |
| C | GS029 | ChargesAndFeatures.tsx | 104 |
| C | GS029 | ChargesAndFeatures.tsx | 147 |
| C | GS029 | IntegrationsTab.tsx | 107 |
| C | GS029 | GeneralTab.tsx | 515 |
| C | GS029 | DeveloperTab.tsx | 440 |
| C | GS029 | DeveloperTab.tsx | 529 |
| C | GS029 | CustomerDetail.tsx | 225 |
| C | GS029 | CustomerDetail.tsx | 244 |
| C | GS029 | CustomerDetail.tsx | 280 |
| C | GS029 | CustomerDetail.tsx | 299 |
| C | GS029 | CustomerSubscriptionView.tsx | 859 |
| C | GS029 | AddonDetails.tsx | 70 |
| C | GS029 | ViewAddOns.tsx | 41 |
| C | GS029 | ViewAddOns.tsx | 85 |
| C | GS029 | CreateAddOns.tsx | 266 |
| C | GS029 | CreateAddOns.tsx | 315 |
| C | GS029 | CreateAddOns.tsx | 501 |
| C | GS029 | CreateAddOns.tsx | 532 |
| C | GS029 | CreateBacktest.tsx | 212 |
| C | GS029 | ViewPlans.tsx | 414 |
| C | GS029 | ViewExperiments.tsx | 47 |
| C | GS029 | ExperimentResults.tsx | 273 |
| C | GS029 | ViewCustomers.tsx | 90 |
| C | GS029 | pyproject.toml | 61 |
| H | GS025 | renovate.json | 0 |
| H | GS025 | package.json | 0 |
| H | GS025 | docker-compose.prod.yaml | 0 |
| H | GS025 | .pre-commit-config.yaml | 0 |
| H | GS025 | docker-compose.dev.yaml | 0 |
| H | GS025 | app.json | 0 |
| H | GS002 | nginx.conf | 0 |
| H | GS002 | nginx.conf | 0 |
| I | GS007 | views.py | 2171 |
| H | GS007 | demos.py | 1144 |
| H | GS007 | demos.py | 1165 |
| H | GS007 | demos.py | 2345 |
| H | GS007 | consumer.py | 69 |
| s | GS009 |  | 0 |
| L | GS012 | model_serializers.py | 906 |
| L | GS012 | model_serializers.py | 1447 |
| L | GS012 | model_serializers.py | 1848 |
| L | GS012 | model_serializers.py | 2421 |
| L | GS012 | model_serializers.py | 2795 |
| L | GS012 | views.py | 291 |
| L | GS012 | views.py | 1196 |
| L | GS012 | views.py | 1202 |
| L | GS012 | views.py | 1237 |
| L | GS012 | views.py | 1838 |
| L | GS012 | billable_metrics.py | 228 |
| L | GS012 | demos.py | 111 |
| L | GS012 | demos.py | 112 |
| L | GS012 | demos.py | 251 |
| L | GS012 | demos.py | 280 |
| L | GS012 | demos.py | 309 |
| L | GS012 | demos.py | 338 |
| L | GS012 | demos.py | 380 |
| L | GS012 | demos.py | 422 |
| L | GS012 | demos.py | 464 |
| L | GS012 | demos.py | 630 |
| L | GS012 | demos.py | 639 |
| L | GS012 | demos.py | 691 |
| L | GS012 | demos.py | 692 |
| L | GS012 | demos.py | 849 |
| L | GS012 | demos.py | 884 |
| L | GS012 | demos.py | 919 |
| L | GS012 | demos.py | 961 |
| L | GS012 | demos.py | 1003 |
| L | GS012 | demos.py | 1045 |
| L | GS012 | demos.py | 1220 |
| L | GS012 | demos.py | 1230 |
| L | GS012 | demos.py | 1277 |
| L | GS012 | demos.py | 1278 |
| L | GS012 | demos.py | 1392 |
| L | GS012 | demos.py | 1478 |
| L | GS012 | demos.py | 1481 |
| L | GS012 | demos.py | 1513 |
| L | GS012 | demos.py | 1514 |
| L | GS012 | demos.py | 1572 |
| L | GS012 | demos.py | 2355 |
| L | GS012 | demos.py | 2363 |
| L | GS012 | demos.py | 2707 |
| L | GS012 | invoice.py | 152 |
| L | GS012 | invoice.py | 302 |
| L | GS012 | invoice.py | 766 |
| L | GS012 | invoice.py | 792 |
| L | GS012 | invoice_pdf.py | 135 |
| L | GS012 | invoice_pdf.py | 589 |
| L | GS012 | initadmin.py | 28 |
| L | GS012 | postman_ci_outputs.py | 146 |
| L | GS012 | postman_ci_outputs.py | 147 |
| L | GS012 | models.py | 352 |
| L | GS012 | models.py | 383 |
| L | GS012 | models.py | 397 |
| L | GS012 | models.py | 455 |
| L | GS012 | models.py | 959 |
| L | GS012 | models.py | 994 |
| L | GS012 | models.py | 1007 |
| L | GS012 | models.py | 1317 |
| L | GS012 | models.py | 1380 |
| L | GS012 | models.py | 1388 |
| L | GS012 | models.py | 1979 |
| L | GS012 | models.py | 3023 |
| L | GS012 | models.py | 3177 |
| L | GS012 | models.py | 3194 |
| L | GS012 | models.py | 3327 |
| L | GS012 | models.py | 3344 |
| L | GS012 | models.py | 3359 |
| L | GS012 | models.py | 3388 |
| L | GS012 | models.py | 3391 |
| L | GS012 | models.py | 3528 |
| L | GS012 | models.py | 3534 |
| L | GS012 | models.py | 3615 |
| L | GS012 | models.py | 3955 |
| L | GS012 | payment_processors.py | 258 |
| L | GS012 | payment_processors.py | 263 |
| L | GS012 | payment_processors.py | 277 |
| L | GS012 | payment_processors.py | 282 |
| L | GS012 | payment_processors.py | 373 |
| L | GS012 | payment_processors.py | 445 |
| L | GS012 | payment_processors.py | 487 |
| L | GS012 | payment_processors.py | 534 |
| L | GS012 | payment_processors.py | 636 |
| L | GS012 | payment_processors.py | 744 |
| L | GS012 | payment_processors.py | 749 |
| L | GS012 | payment_processors.py | 829 |
| L | GS012 | payment_processors.py | 941 |
| L | GS012 | payment_processors.py | 1036 |
| L | GS012 | payment_processors.py | 1138 |
| L | GS012 | model_serializers.py | 522 |
| L | GS012 | model_serializers.py | 579 |
| L | GS012 | model_serializers.py | 663 |
| L | GS012 | model_serializers.py | 757 |
| L | GS012 | model_serializers.py | 1087 |
| L | GS012 | model_serializers.py | 1384 |
| L | GS012 | user.py | 84 |
| L | GS012 | tasks.py | 63 |
| L | GS012 | tasks.py | 80 |
| L | GS012 | tasks.py | 215 |
| L | GS012 | tasks.py | 320 |
| L | GS012 | tasks.py | 324 |
| L | GS012 | tasks.py | 502 |
| L | GS012 | tasks.py | 505 |
| L | GS012 | tasks.py | 547 |
| L | GS012 | auth_views.py | 494 |
| L | GS012 | crm_views.py | 73 |
| L | GS012 | crm_views.py | 195 |
| L | GS012 | crm_views.py | 242 |
| L | GS012 | crm_views.py | 339 |
| L | GS012 | crm_views.py | 439 |
| L | GS012 | crm_views.py | 449 |
| L | GS012 | model_views.py | 287 |
| L | GS012 | model_views.py | 965 |
| L | GS012 | model_views.py | 1041 |
| L | GS012 | model_views.py | 1079 |
| L | GS012 | model_views.py | 1124 |
| L | GS012 | model_views.py | 1345 |
| L | GS012 | model_views.py | 1707 |
| L | GS012 | model_views.py | 1843 |
| L | GS012 | model_views.py | 2354 |
| L | GS012 | model_views.py | 2513 |
| L | GS012 | organization_views.py | 56 |
| L | GS012 | organization_views.py | 103 |
| L | GS012 | views.py | 317 |
| L | GS012 | webhook_views.py | 35 |
| L | GS012 | webhook_views.py | 52 |
| H | GS014 | docker-compose.dev.yaml | 41 |
| H | GS014 | docker-compose.prod.yaml | 17 |
| H | GS017 | authn.go | 26 |
| H | GS018 | views.py | 1021 |
| H | GS018 | views.py | 1266 |
| H | GS018 | views.py | 1359 |
| H | GS018 | invoice.py | 445 |
| H | GS018 | models.py | 3161 |
| H | GS018 | models.py | 3598 |
| H | GS018 | payment_processors.py | 1364 |
| H | GS018 | views.py | 459 |
| H | GS019 | model_backend.py | 14 |
| M | GS019 | payment_processors.py | 104 |
| M | GS019 | payment_processors.py | 397 |
| M | GS019 | payment_processors.py | 1158 |
| M | GS019 | user.py | 68 |
| c | GS021 |  | 2231 |
| c | GS021 |  | 691 |
| s | GS021 |  | 45 |
| s | GS021 |  | 208 |
| s | GS021 |  | 285 |
| s | GS021 |  | 334 |
| s | GS021 |  | 517 |
| s | GS021 |  | 733 |
| c | GS021 |  | 56 |
| s | GS021 |  | 20 |
| s | GS021 |  | 35 |
| s | GS021 |  | 38 |
| s | GS021 |  | 45 |
| s | GS021 |  | 61 |
| s | GS021 |  | 75 |
| s | GS021 |  | 94 |
| s | GS021 |  | 124 |
| s | GS021 |  | 144 |
| s | GS021 |  | 165 |
| s | GS021 |  | 73 |
| s | GS021 |  | 116 |
| s | GS021 |  | 15 |
| s | GS021 |  | 19 |
| s | GS021 |  | 28 |
| r | GS022 |  | 16 |
| r | GS022 |  | 14 |
| r | GS022 |  | 15 |
| r | GS022 |  | 30 |
| r | GS022 |  | 38 |
| r | GS022 |  | 268 |
| r | GS022 |  | 93 |
| r | GS022 |  | 30 |
| r | GS022 |  | 33 |
| r | GS022 |  | 83 |
| r | GS022 |  | 129 |
| r | GS022 |  | 169 |
| r | GS022 |  | 220 |
| r | GS022 |  | 365 |
| r | GS022 |  | 459 |
| r | GS022 |  | 1672 |
| r | GS022 |  | 1674 |
| r | GS022 |  | 617 |
| r | GS022 |  | 638 |
| r | GS022 |  | 73 |
| r | GS022 |  | 4101 |
| r | GS022 |  | 4130 |
| r | GS022 |  | 166 |
| r | GS022 |  | 648 |
| r | GS022 |  | 1150 |
| r | GS022 |  | 149 |
| r | GS022 |  | 172 |
| r | GS022 |  | 20 |
| r | GS022 |  | 271 |
| r | GS022 |  | 341 |
| r | GS022 |  | 686 |
| r | GS022 |  | 33 |
| r | GS022 |  | 1843 |
| r | GS022 |  | 1852 |
| r | GS022 |  | 1856 |
| r | GS022 |  | 1986 |
| r | GS022 |  | 1993 |
| r | GS022 |  | 1997 |
| r | GS022 |  | 38 |
| r | GS022 |  | 54 |
| r | GS022 |  | 55 |
| r | GS022 |  | 10 |
| r | GS022 |  | 9 |
| r | GS022 |  | 51 |
| r | GS022 |  | 57 |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-debug_mode |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | YAML-ECB85AD8 | settings.py | ? |
| ? | YAML-B39DC08C | postman_ci_outputs.py | ? |
| ? | YAML-B39DC08C | utils.py | ? |

---
*Сгенерировано GSC v0.6 · 2026-08-10T14:29:15.117501*
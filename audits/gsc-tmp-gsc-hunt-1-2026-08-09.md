---
title: "GSC Audit: /tmp/gsc-hunt-1"
date: 2026-08-09
tags: [gsc, audit, security]
---

# 🔒 GSC Audit — /tmp/gsc-hunt-1

**Дата:** 09.08.2026 12:01  
**Путь:** `/tmp/gsc-hunt-1`  
**Всего находок:** 922  
**CRITICAL:** 139 | **HIGH:** 40 | **MEDIUM:** 334 | **LOW:** 247

## 📊 По детекторам

| Детектор | Находок |
|----------|--------|
| GS029 | 266 |
| GS000-LEGACY | 205 |
| GS018 | 101 |
| GS025 | 49 |
| GS003 | 46 |
| GS034-token_collector | 41 |
| GS037-hardcoded_password | 37 |
| GS005 | 33 |
| GS022 | 28 |
| GS007 | 24 |
| GS012 | 19 |
| GS010 | 14 |
| GS001 | 10 |
| GS021 | 9 |
| GS025-hardcoded_secret | 6 |
| GS025-eval_usage | 6 |
| GS008 | 5 |
| GS017 | 4 |
| GS020 | 3 |
| GS015 | 2 |
| GS037-hardcoded_api_key | 2 |
| GS037-high_risk | 2 |
| GS016 | 2 |
| GS019 | 2 |
| GS036-dangerously_set_html | 1 |
| GS002 | 1 |
| GS009 | 1 |
| GS011 | 1 |
| GS014 | 1 |
| Rust: .clone() in hot path | 1 |

## 🔴 Критические и важные

| Категория | Правило | Файл | Строка | Детали |
|-----------|--------|------|--------|--------|
| CRITICAL | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 186 | OWASP A03: Injection |
| CRITICAL | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 | OWASP A03: Injection |
| CRITICAL | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 53 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 393 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | 62c7711123a8_french_email_templates.py | 367 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 | String concatenation with SQL — classic SQL injection vector |
| CRITICAL | GS001 | generator.py | 12 | Found: API_KEY = 'sk_LexJK2eK0jY3Kmm9gE6R6nJ4M8RwrZpN' |
| CRITICAL | GS001 | tests.py | 114 | Found: password='abcd' |
| CRITICAL | GS001 | tests.py | 133 | Found: password='abcd' |
| CRITICAL | GS001 | tests.py | 151 | Found: password='abcd' |
| CRITICAL | GS001 | tests.py | 242 | Found: password='abcd' |
| CRITICAL | GS001 | tests.py | 319 | Found: password= '123456' |
| CRITICAL | GS001 | testing.py | 137 | Found: password='abcd' |
| CRITICAL | GS001 | app.example.yaml | 20 | Found: PASSWORD: 'SMTP_PASSWORD' |
| CRITICAL | GS001 | config.py | 12 | Found: postgres://docker:docker@db/docker |
| CRITICAL | GS001 | prod.example.yaml | 20 | Found: PASSWORD: 'SMTP_PASSWORD' |
| CRITICAL | GS025 | migrate_database.sh | 6 | Match: sudo chmod 777 /cloudsql |
| CRITICAL | GS025 | migrate_database.sh | 6 | Match: sudo chmod 777 /cloudsql |
| CRITICAL | GS029 | 1c3fda18bad6_.py | 410 | Match:     session.query(Event).filter_by(key='indaba2020'). |
| CRITICAL | GS029 | c795c179c2b2_.py | 221 | Match:     event = session.query(Event).filter_by(key='kambu |
| CRITICAL | GS029 | 15d51e2866ce_add_offer_award_email.py | 84 | Match:     op.execute("""DELETE FROM email_template WHERE ke |
| CRITICAL | GS029 | 6d34d1ab6864_eeml_review_form.py | 180 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 78f4d11203c5_ai4d_more_changes.py | 388 | Match:     session.query(EmailTemplate).filter_by(key='confi |
| CRITICAL | GS029 | de12a6f382c1_ai4d_review_form.py | 178 | Match:     event = session.query(Event).filter_by(key='ai4d2 |
| CRITICAL | GS029 | de12a6f382c1_ai4d_review_form.py | 309 | Match:     event = session.query(Event).filter_by(key='ai4d2 |
| CRITICAL | GS029 | bda5cebe15fd_indabax_registration.py | 265 | Match:     event = session.query(Event).filter_by(key='indab |
| CRITICAL | GS029 | bda5cebe15fd_indabax_registration.py | 671 | Match:     event = session.query(Event).filter_by(key='indab |
| CRITICAL | GS029 | 76c9226545bb_update_review_assigned_template.py | 47 | Match:     en = db.session.query(EmailTemplate).filter_by(la |
| CRITICAL | GS029 | 76c9226545bb_update_review_assigned_template.py | 57 | Match:     fr = db.session.query(EmailTemplate).filter_by(la |
| CRITICAL | GS029 | 76c9226545bb_update_review_assigned_template.py | 83 | Match:     fr = db.session.query(EmailTemplate).filter_by(la |
| CRITICAL | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 717 | Match:     q.key = 'review-identifier' |
| CRITICAL | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 724 | Match:     q.key = 'review-identifier' |
| CRITICAL | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 129 | Match:     event = session.query(Event).filter_by(key='indab |
| CRITICAL | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 | Match:     op.execute(f"""DELETE FROM email_template where e |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 21 | Match:         SET key = 'nomination_title' |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 27 | Match:     op.execute("""UPDATE question SET key='nomination |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 28 | Match:     op.execute("""UPDATE question SET key='nomination |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 29 | Match:     op.execute("""UPDATE question SET key='nomination |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 31 | Match:     op.execute("""UPDATE Section SET key='nominee_sec |
| CRITICAL | GS029 | e3e47585f336_section_question_key.py | 32 | Match:     op.execute("""UPDATE Question SET key='nominating |
| CRITICAL | GS029 | 49663ad38428_add_guest_removal_email_template.py | 41 | Match:     op.execute("DELETE FROM email_template WHERE key  |
| CRITICAL | GS029 | 613df2d7a759_update_email_template.py | 18 | Match:     op.execute("""UPDATE email_template SET subject = |
| CRITICAL | GS029 | 613df2d7a759_update_email_template.py | 22 | Match:     op.execute("""UPDATE email_template SET subject = |
| CRITICAL | GS029 | 964ead196cb9_add_miniconf_url.py | 35 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 1e05a293f402_eeml_registration_form.py | 185 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 1e05a293f402_eeml_registration_form.py | 317 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 2279e1fa2e49_eeml_review_update2.py | 187 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 2279e1fa2e49_eeml_review_update2.py | 239 | Match:     event = session.query(Event).filter_by(key='eeml2 |
| CRITICAL | GS029 | 3bc5355f159c_add_org_url_and_event_fields.py | 31 | Match:     op.execute("""UPDATE event SET email_from = 'baob |
| CRITICAL | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 475 | Match:     password_reset_template = session.query(EmailTemp |
| CRITICAL | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 496 | Match:     withdrawal_template = session.query(EmailTemplate |
| CRITICAL | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 279 | Match:     organisation_question.key = 'review-identifier' |
| CRITICAL | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 281 | Match:     country_question.key = 'review-identifier' |
| CRITICAL | GS029 | 3e7bdff8af80_eeml_form_updates.py | 65 | Match:         WHERE key='withdrawal' |
| CRITICAL | GS029 | 70b2a4f4a596_offer_paid_email.py | 71 | Match:     op.execute("""DELETE FROM email_template WHERE ke |
| CRITICAL | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 24 | Match:     op.execute("""UPDATE email_template SET subject=' |
| CRITICAL | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 25 | Match:     op.execute("""UPDATE email_template SET subject=' |
| CRITICAL | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 26 | Match:     op.execute("""UPDATE email_template SET subject=' |
| CRITICAL | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 27 | Match:     op.execute("""UPDATE email_template SET subject=' |
| CRITICAL | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 28 | Match:     op.execute("""UPDATE email_template SET subject=' |
| CRITICAL | GS029 | tests.py | 33 | Match:         event = self.add_event(key='CONN2025') |
| CRITICAL | GS029 | tests.py | 31 | Match:             key='SPEEDNET' |
| CRITICAL | GS029 | tests.py | 52 | Match:         self.event = self.add_event({'en': 'Event Wit |
| CRITICAL | GS029 | tests.py | 63 | Match:         self.event_with_nomination = self.add_event({ |
| CRITICAL | GS029 | tests.py | 25 | Match:         event = self.add_event(key='DISC2026') |
| CRITICAL | GS029 | tests.py | 497 | Match:         other_event = self.add_event(key='DISC2027') |
| CRITICAL | GS029 | tests.py | 1287 | Match:         question1.key = 'review-identifier' |
| CRITICAL | GS029 | tests.py | 1291 | Match:         question2.key = 'review-identifier' |
| CRITICAL | GS029 | tests.py | 1763 | Match:             key='review-identifier') |
| CRITICAL | GS029 | tests.py | 1772 | Match:             key='review-identifier') |
| CRITICAL | GS029 | tests.py | 2001 | Match:             key='review-identifier') |
| CRITICAL | GS029 | tests.py | 2010 | Match:             key='review-identifier') |
| CRITICAL | GS029 | tests.py | 2219 | Match:         no_form_event = self.add_event(key="no_form_e |
| CRITICAL | GS029 | tests.py | 38 | Match:         event = self.add_event(key='TEST2025') |
| CRITICAL | GS029 | tests.py | 396 | Match:         other_event = self.add_event(key='OTHERTAGEVE |
| CRITICAL | GS029 | tests.py | 540 | Match:         event = self.add_event(key='FRTEST2025', orga |
| CRITICAL | GS029 | tests.py | 636 | Match:         other_event = self.add_event(key='OTHEREVENT2 |
| CRITICAL | GS029 | tests.py | 677 | Match:         event = self.add_event(key='QUEUE2025') |
| CRITICAL | GS029 | tests.py | 20 | Match:         event = self.add_event(key='OUTBOX2025') |
| CRITICAL | GS029 | tests.py | 100 | Match:         message.claim_token = 'abandoned' |
| CRITICAL | GS029 | tests.py | 57 | Match:             key='SPEEDNET' |
| CRITICAL | GS029 | tests.py | 229 | Match:                 key='SPEEDNET' |
| CRITICAL | GS029 | tests.py | 23 | Match:             key='INDABA2026' |
| CRITICAL | GS029 | tests.py | 648 | Match:             key='INDABAFR2026', |
| CRITICAL | GS029 | tests.py | 320 | Match:         user.verify_token = 'existing token' |
| CRITICAL | GS029 | tests.py | 32 | Match:         nomination_event = self.add_event(key="AWARD_ |
| CRITICAL | GS029 | tests.py | 44 | Match:             Section(nomination_event.id, 1, key='nomi |
| CRITICAL | GS029 | tests.py | 57 | Match:         questions[0].key = 'nominating_capacity' |
| CRITICAL | GS029 | tests.py | 58 | Match:         questions[2].key = 'nomination_title' |
| CRITICAL | GS029 | tests.py | 59 | Match:         questions[3].key = 'nomination_firstname' |
| CRITICAL | GS029 | tests.py | 60 | Match:         questions[4].key = 'nomination_lastname' |
| CRITICAL | GS029 | tests.py | 61 | Match:         questions[5].key = 'nomination_email' |
| CRITICAL | GS029 | tests.py | 926 | Match:         self.event2 = self.add_event({'en': 'Second e |
| CRITICAL | GS029 | tests.py | 1357 | Match:         self.event = self.add_event(key='TESTEVENT') |
| CRITICAL | GS029 | tests.py | 1957 | Match:         self.event = self.add_event(key='SURVEYEVENT' |
| CRITICAL | GS029 | tests.py | 1958 | Match:         self.other_event = self.add_event({'en': 'Oth |
| CRITICAL | GS029 | tests.py | 1977 | Match:     def _get_event_by_key(self, key='SURVEYEVENT'): |
| CRITICAL | GS029 | tests.py | 41 | Match:             key='SPEEDNET' |
| CRITICAL | GS029 | AttendanceTable.js | 525 | Match:         <div className="bg-white rounded-2xl shadow-s |
| CRITICAL | GS029 | TagConfigComponent.js | 230 | Match:       <div className="space-y-6 p-6 bg-slate-50/50 ro |
| CRITICAL | GS029 | TagConfigComponent.js | 300 | Match:         <div className="flex flex-col md:flex-row ite |
| CRITICAL | GS029 | TagConfigComponent.js | 379 | Match:       <div key='card-container' className="w-full pt- |
| CRITICAL | GS029 | TagConfigComponent.js | 380 | Match:         <div className="bg-white rounded-2xl shadow-s |
| CRITICAL | GS029 | InvitedGuestComponent.js | 468 | Match:         <div className="bg-white rounded-2xl shadow-s |
| CRITICAL | GS029 | ResponseListComponent.js | 271 | Match:                 <div className="bg-white rounded-2xl  |
| CRITICAL | GS029 | OfferAdminComponent.js | 403 | Match:                 <div className="bg-white rounded-2xl  |
| CRITICAL | GS029 | ReferenceComponent.js | 117 | Match:                         key="fileupload" /> |
| CRITICAL | GS029 | InvoiceAdminListComponent.js | 243 | Match:                     <Trans key="confirmInvoicePaid">A |
| CRITICAL | GS029 | InvoiceAdminListComponent.js | 254 | Match:                     <Trans key="confirmInvoiceCancel" |
| CRITICAL | GS005 | 02242641e122_add_local_event.py | 190 | Line 190: op.get_bind().execute("""UPDATE question SET is_re |
| CRITICAL | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 186 | Line 186: op.execute(f"""DELETE FROM email_template where ev |
| CRITICAL | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 | Line 187: op.execute(f"""DELETE FROM email_template where ev |
| CRITICAL | GS005 | 1349a2c924f4_.py | 282 | Line 282: op.get_bind().execute('DELETE FROM review_question |
| CRITICAL | GS005 | 1c3fda18bad6_.py | 405 | Line 405: op.get_bind().execute("""UPDATE Section SET depend |
| CRITICAL | GS005 | 1e05a293f402_eeml_registration_form.py | 320 | Line 320: op.execute("""DELETE FROM registration_question WH |
| CRITICAL | GS005 | 1e05a293f402_eeml_registration_form.py | 321 | Line 321: op.execute("""DELETE FROM registration_section WHE |
| CRITICAL | GS005 | 1e05a293f402_eeml_registration_form.py | 322 | Line 322: op.execute("""DELETE FROM registration_form WHERE  |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 53 | Line 53: op.execute("""DELETE FROM email_template WHERE lang |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 53 | Line 53: op.execute("""DELETE FROM email_template WHERE lang |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 393 | Line 393: op.execute("""DELETE FROM email_template WHERE lan |
| CRITICAL | GS005 | 2241922a3305_redo_french_email_templates.py | 393 | Line 393: op.execute("""DELETE FROM email_template WHERE lan |
| CRITICAL | GS005 | 3ab678fc66cd_populate_reg_form.py | 435 | Line 435: op.get_bind().execute('DELETE FROM registration_qu |
| CRITICAL | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 340 | Line 340: op.execute("""DELETE FROM Answer WHERE question_id |
| CRITICAL | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 347 | Line 347: op.execute("""DELETE FROM Answer WHERE question_id |
| CRITICAL | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 354 | Line 354: op.execute("""DELETE FROM Answer WHERE question_id |
| CRITICAL | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 | Line 288: op.execute("""DELETE FROM email_template WHERE key |
| CRITICAL | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 | Line 288: op.execute("""DELETE FROM email_template WHERE key |
| CRITICAL | GS005 | 62c7711123a8_french_email_templates.py | 367 | Line 367: op.execute("""DELETE FROM email_template WHERE lan |
| CRITICAL | GS005 | 62c7711123a8_french_email_templates.py | 367 | Line 367: op.execute("""DELETE FROM email_template WHERE lan |
| CRITICAL | GS005 | 964ead196cb9_add_miniconf_url.py | 36 | Line 36: op.execute("""UPDATE event SET miniconf_url = 'mini |
| CRITICAL | GS005 | bda5cebe15fd_indabax_registration.py | 674 | Line 674: op.execute("""DELETE FROM registration_question WH |
| CRITICAL | GS005 | bda5cebe15fd_indabax_registration.py | 675 | Line 675: op.execute("""DELETE FROM registration_section WHE |
| CRITICAL | GS005 | bda5cebe15fd_indabax_registration.py | 676 | Line 676: op.execute("""DELETE FROM registration_form WHERE  |
| CRITICAL | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 | Line 69: op.execute("""DELETE FROM email_template WHERE key  |
| CRITICAL | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 | Line 69: op.execute("""DELETE FROM email_template WHERE key  |
| CRITICAL | GS016 | migrate_database.sh | 6 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS016 | migrate_database.sh | 6 | SUID binary outside standard system paths — potential privil |
| CRITICAL | GS019 | testing.py | 174 | Session/JWT secret hardcoded in source. Anyone with code acc |
| HIGH | GS000-LEGACY | api.py | 235 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 153 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 167 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 220 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 228 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 259 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 615 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 68 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 178 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 230 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 286 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 528 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 155 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 330 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 355 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 74 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 223 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 230 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 255 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 318 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 371 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 381 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | service.py | 94 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | tests.py | 138 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 803 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 823 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | api.py | 861 | File upload without MIME-type validation → malicious file up |
| HIGH | GS000-LEGACY | config.py | 12 | Redteam Kit |
| HIGH | GS025 | storage.py | 28 |  |
| HIGH | GS025 | package-lock.json | 0 | Permissions 664 — should be 600 |
| HIGH | GS025 | docker-compose.yml | 0 | Permissions 664 — should be 600 |
| HIGH | GS002 | nginx.conf | 0 | File nginx.conf has permissions -rw-rw-r-- — readable by any |
| HIGH | GS011 | testing.py | 174 | Found JWT secret in code: 'webhook_...'. JWT secrets must be |
| HIGH | GS014 | config.py | 12 | Database URL contains password in plaintext. Use environment |
| HIGH | GS017 | api.py | 221 | Password length = 4 chars. |
| HIGH | GS017 | api.py | 265 | Password length = 4 chars. |
| HIGH | GS017 | util.js | 700 | Password length = 3 chars. |
| HIGH | GS017 | DiscussionSpaces.js | 175 | Password length = 4 chars. |
| HIGH | GS018 | api.py | 268 | Float arithmetic for money leads to rounding errors exploita |
| HIGH | ? | sw.js | 46 | Clone in performance-critical code — consider references |

## 📋 Все находки

| Кат. | Правило | Файл | Строка |
|------|--------|------|--------|
| C | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 186 |
| C | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 |
| M | GS010 | api.py | 135 |
| M | GS010 | api.py | 68 |
| M | GS010 | api.py | 124 |
| M | GS010 | api.py | 143 |
| M | GS010 | api.py | 180 |
| M | GS010 | api.py | 241 |
| M | GS010 | api.py | 275 |
| M | GS010 | api.py | 293 |
| M | GS010 | api.py | 264 |
| M | GS010 | misc.py | 16 |
| M | GS010 | api.py | 101 |
| M | GS010 | api.py | 194 |
| M | GS010 | api.py | 643 |
| M | GS010 | api.py | 299 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| L | GS000-LEGACY | strings.py | 8 |
| L | GS000-LEGACY | tests.py | 520 |
| L | GS000-LEGACY | service.py | 90 |
| M | GS018 | config.py | 15 |
| M | GS018 | tests.py | 1149 |
| M | GS018 | tests.py | 1150 |
| M | GS018 | tests.py | 69 |
| M | GS018 | tests.py | 70 |
| M | GS018 | tests.py | 75 |
| M | GS018 | tests.py | 78 |
| M | GS018 | tests.py | 97 |
| M | GS018 | tests.py | 98 |
| M | GS018 | tests.py | 99 |
| M | GS018 | tests.py | 100 |
| M | GS018 | tests.py | 134 |
| M | GS018 | tests.py | 139 |
| M | GS018 | tests.py | 142 |
| M | GS018 | tests.py | 147 |
| M | GS018 | tests.py | 150 |
| M | GS018 | tests.py | 156 |
| M | GS018 | tests.py | 163 |
| M | GS018 | tests.py | 169 |
| M | GS018 | tests.py | 175 |
| M | GS018 | tests.py | 182 |
| M | GS018 | tests.py | 185 |
| M | GS018 | tests.py | 221 |
| M | GS018 | tests.py | 227 |
| M | GS018 | tests.py | 234 |
| M | GS018 | tests.py | 239 |
| M | GS018 | tests.py | 249 |
| M | GS018 | tests.py | 255 |
| M | GS018 | tests.py | 262 |
| M | GS018 | tests.py | 267 |
| M | GS018 | tests.py | 275 |
| M | GS018 | tests.py | 281 |
| M | GS018 | tests.py | 288 |
| M | GS018 | tests.py | 298 |
| M | GS018 | tests.py | 301 |
| M | GS018 | tests.py | 302 |
| M | GS018 | tests.py | 309 |
| M | GS018 | tests.py | 316 |
| M | GS018 | tests.py | 93 |
| M | GS018 | tests.py | 94 |
| M | GS018 | tests.py | 102 |
| M | GS018 | tests.py | 108 |
| M | GS018 | tests.py | 115 |
| M | GS018 | tests.py | 116 |
| M | GS018 | tests.py | 176 |
| M | GS018 | tests.py | 177 |
| M | GS018 | tests.py | 178 |
| M | GS018 | tests.py | 179 |
| M | GS018 | tests.py | 180 |
| M | GS018 | tests.py | 181 |
| M | GS018 | tests.py | 182 |
| M | GS018 | tests.py | 183 |
| M | GS018 | tests.py | 184 |
| M | GS018 | tests.py | 199 |
| M | GS018 | tests.py | 200 |
| M | GS018 | tests.py | 201 |
| M | GS018 | tests.py | 202 |
| M | GS018 | tests.py | 203 |
| M | GS018 | tests.py | 204 |
| M | GS018 | tests.py | 205 |
| M | GS018 | tests.py | 206 |
| M | GS018 | tests.py | 207 |
| M | GS018 | tests.py | 234 |
| M | GS018 | tests.py | 235 |
| M | GS018 | tests.py | 236 |
| M | GS018 | tests.py | 237 |
| M | GS018 | tests.py | 238 |
| M | GS018 | tests.py | 239 |
| M | GS018 | tests.py | 240 |
| M | GS018 | tests.py | 241 |
| M | GS018 | tests.py | 242 |
| M | GS018 | tests.py | 271 |
| M | GS018 | tests.py | 272 |
| M | GS018 | tests.py | 273 |
| M | GS018 | tests.py | 274 |
| M | GS018 | tests.py | 275 |
| M | GS018 | tests.py | 276 |
| M | GS018 | tests.py | 277 |
| M | GS018 | tests.py | 278 |
| M | GS018 | generator.py | 25 |
| M | GS018 | generator.py | 26 |
| M | GS018 | generator.py | 27 |
| M | GS018 | generator.py | 28 |
| M | GS018 | generator.py | 29 |
| M | GS018 | generator.py | 30 |
| M | GS018 | generator.py | 31 |
| M | GS018 | generator.py | 32 |
| M | GS018 | generator.py | 33 |
| M | GS018 | generator.py | 34 |
| M | GS018 | generator.py | 35 |
| M | GS018 | generator.py | 36 |
| M | GS018 | generator.py | 37 |
| M | GS018 | generator.py | 38 |
| M | GS018 | generator.py | 39 |
| M | GS018 | generator.py | 40 |
| M | GS018 | generator.py | 41 |
| M | GS018 | generator.py | 42 |
| M | GS018 | generator.py | 43 |
| M | GS018 | generator.py | 44 |
| M | GS018 | generator.py | 45 |
| C | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 53 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 393 |
| C | GS005 | 62c7711123a8_french_email_templates.py | 367 |
| C | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 |
| H | GS000-LEGACY | api.py | 235 |
| H | GS000-LEGACY | api.py | 153 |
| H | GS000-LEGACY | api.py | 167 |
| H | GS000-LEGACY | api.py | 220 |
| H | GS000-LEGACY | api.py | 228 |
| H | GS000-LEGACY | api.py | 259 |
| H | GS000-LEGACY | api.py | 615 |
| H | GS000-LEGACY | api.py | 68 |
| H | GS000-LEGACY | api.py | 178 |
| H | GS000-LEGACY | api.py | 230 |
| H | GS000-LEGACY | api.py | 286 |
| H | GS000-LEGACY | api.py | 528 |
| H | GS000-LEGACY | tests.py | 155 |
| H | GS000-LEGACY | tests.py | 330 |
| H | GS000-LEGACY | tests.py | 355 |
| H | GS000-LEGACY | api.py | 74 |
| H | GS000-LEGACY | api.py | 223 |
| H | GS000-LEGACY | api.py | 230 |
| H | GS000-LEGACY | api.py | 255 |
| H | GS000-LEGACY | api.py | 318 |
| H | GS000-LEGACY | api.py | 371 |
| H | GS000-LEGACY | api.py | 381 |
| H | GS000-LEGACY | service.py | 94 |
| H | GS000-LEGACY | tests.py | 138 |
| H | GS000-LEGACY | api.py | 803 |
| H | GS000-LEGACY | api.py | 823 |
| H | GS000-LEGACY | api.py | 861 |
| H | GS000-LEGACY | config.py | 12 |
| H | GS025 | storage.py | 28 |
| M | GS025 | tests.py | 47 |
| M | GS025 | tests.py | 48 |
| M | GS025 | tests.py | 49 |
| M | GS025 | tests.py | 50 |
| M | GS025 | tests.py | 51 |
| M | GS025 | tests.py | 52 |
| M | GS025 | tests.py | 53 |
| M | GS025 | tests.py | 54 |
| M | GS025 | tests.py | 55 |
| M | GS025 | tests.py | 56 |
| M | GS025 | testing.py | 116 |
| M | GS025 | testing.py | 137 |
| M | GS025 | testing.py | 300 |
| M | GS025 | tests.py | 100 |
| M | GS025 | tests.py | 162 |
| M | GS025 | tests.py | 181 |
| M | GS025 | tests.py | 196 |
| M | GS025 | tests.py | 233 |
| M | GS025 | tests.py | 261 |
| M | GS025 | tests.py | 319 |
| M | GS025 | tests.py | 320 |
| M | GS025 | tests.py | 332 |
| M | GS025 | tests.py | 333 |
| M | GS025 | tests.py | 334 |
| M | GS025 | tests.py | 335 |
| M | GS025 | tests.py | 740 |
| M | GS025 | tests.py | 741 |
| M | GS025 | tests.py | 742 |
| M | GS025 | tests.py | 743 |
| M | GS025 | tests.py | 744 |
| M | GS025 | tests.py | 812 |
| M | GS025 | tests.py | 813 |
| M | GS025 | tests.py | 814 |
| M | GS025 | tests.py | 867 |
| M | GS025 | tests.py | 868 |
| M | GS025 | tests.py | 869 |
| M | GS025 | tests.py | 608 |
| M | GS025 | tests.py | 613 |
| M | GS025 | tests.py | 1509 |
| M | GS025 | tests.py | 1673 |
| M | GS025 | tests.py | 114 |
| M | GS025 | tests.py | 133 |
| M | GS025 | tests.py | 151 |
| M | GS025 | tests.py | 242 |
| M | GS029 | 1c3fda18bad6_.py | 410 |
| M | GS029 | c795c179c2b2_.py | 221 |
| M | GS029 | 15d51e2866ce_add_offer_award_email.py | 84 |
| M | GS029 | cb503c2afd08_ai4d_fixes.py | 298 |
| M | GS029 | 6d34d1ab6864_eeml_review_form.py | 180 |
| M | GS029 | 78f4d11203c5_ai4d_more_changes.py | 318 |
| M | GS029 | 78f4d11203c5_ai4d_more_changes.py | 388 |
| M | GS029 | de12a6f382c1_ai4d_review_form.py | 178 |
| M | GS029 | de12a6f382c1_ai4d_review_form.py | 309 |
| M | GS029 | bda5cebe15fd_indabax_registration.py | 265 |
| M | GS029 | bda5cebe15fd_indabax_registration.py | 671 |
| M | GS029 | 76c9226545bb_update_review_assigned_template.py | 47 |
| M | GS029 | 76c9226545bb_update_review_assigned_template.py | 57 |
| M | GS029 | 76c9226545bb_update_review_assigned_template.py | 83 |
| M | GS029 | ea987b257ee0_ai4d_updates.py | 342 |
| M | GS029 | 43597f3ea193_redo_ai4d_call.py | 399 |
| M | GS029 | 43597f3ea193_redo_ai4d_call.py | 418 |
| M | GS029 | 43597f3ea193_redo_ai4d_call.py | 420 |
| M | GS029 | 43597f3ea193_redo_ai4d_call.py | 438 |
| M | GS029 | 6b64b8037b7b_prc_review_update2.py | 480 |
| M | GS029 | 347a14922cff_ai4d_prc_review_form.py | 419 |
| M | GS029 | 347a14922cff_ai4d_prc_review_form.py | 1385 |
| M | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 531 |
| M | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 717 |
| M | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 724 |
| M | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 730 |
| M | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 129 |
| M | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 186 |
| M | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 |
| M | GS029 | e3e47585f336_section_question_key.py | 21 |
| M | GS029 | e3e47585f336_section_question_key.py | 27 |
| M | GS029 | e3e47585f336_section_question_key.py | 28 |
| M | GS029 | e3e47585f336_section_question_key.py | 29 |
| M | GS029 | e3e47585f336_section_question_key.py | 31 |
| M | GS029 | e3e47585f336_section_question_key.py | 32 |
| M | GS029 | 49663ad38428_add_guest_removal_email_template.py | 41 |
| M | GS029 | ca538998737f_add_ai4d_first_call.py | 417 |
| M | GS029 | 613df2d7a759_update_email_template.py | 18 |
| M | GS029 | 613df2d7a759_update_email_template.py | 22 |
| M | GS029 | 039addb92a03_ai4d_call_launch.py | 298 |
| M | GS029 | 964ead196cb9_add_miniconf_url.py | 35 |
| M | GS029 | 1e05a293f402_eeml_registration_form.py | 185 |
| M | GS029 | 1e05a293f402_eeml_registration_form.py | 317 |
| M | GS029 | 2279e1fa2e49_eeml_review_update2.py | 187 |
| M | GS029 | 2279e1fa2e49_eeml_review_update2.py | 239 |
| M | GS029 | 3bc5355f159c_add_org_url_and_event_fields.py | 31 |
| M | GS029 | 4b5d67699684_ai4d_scholarship_call_updates.py | 298 |
| M | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 475 |
| M | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 496 |
| M | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 276 |
| M | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 279 |
| M | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 281 |
| M | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 286 |
| M | GS029 | 3e7bdff8af80_eeml_form_updates.py | 65 |
| M | GS029 | 70b2a4f4a596_offer_paid_email.py | 71 |
| M | GS029 | 49d55031108e_ai4d_scholarships.py | 417 |
| M | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 24 |
| M | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 25 |
| M | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 26 |
| M | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 27 |
| M | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 28 |
| M | GS029 | api.py | 748 |
| M | GS029 | tests.py | 33 |
| M | GS029 | tests.py | 31 |
| M | GS029 | tests.py | 13 |
| M | GS029 | tests.py | 14 |
| M | GS029 | tests.py | 52 |
| M | GS029 | tests.py | 63 |
| M | GS029 | tests.py | 173 |
| M | GS029 | tests.py | 479 |
| M | GS029 | tests.py | 480 |
| M | GS029 | tests.py | 665 |
| M | GS029 | tests.py | 887 |
| M | GS029 | tests.py | 997 |
| M | GS029 | tests.py | 25 |
| M | GS029 | tests.py | 497 |
| M | GS029 | tests.py | 47 |
| M | GS029 | tests.py | 48 |
| M | GS029 | tests.py | 49 |
| M | GS029 | tests.py | 50 |
| M | GS029 | tests.py | 51 |
| M | GS029 | tests.py | 52 |
| M | GS029 | tests.py | 53 |
| M | GS029 | tests.py | 54 |
| M | GS029 | tests.py | 55 |
| M | GS029 | tests.py | 56 |
| M | GS029 | tests.py | 1269 |
| M | GS029 | tests.py | 1270 |
| M | GS029 | tests.py | 1287 |
| M | GS029 | tests.py | 1291 |
| M | GS029 | tests.py | 1416 |
| M | GS029 | tests.py | 1417 |
| M | GS029 | tests.py | 1753 |
| M | GS029 | tests.py | 1763 |
| M | GS029 | tests.py | 1772 |
| M | GS029 | tests.py | 1991 |
| M | GS029 | tests.py | 2001 |
| M | GS029 | tests.py | 2010 |
| M | GS029 | tests.py | 2219 |
| M | GS029 | tests.py | 2603 |
| M | GS029 | tests.py | 38 |
| M | GS029 | tests.py | 396 |
| M | GS029 | tests.py | 540 |
| M | GS029 | tests.py | 636 |
| M | GS029 | tests.py | 677 |
| M | GS029 | tests.py | 32 |
| M | GS029 | testing.py | 116 |
| M | GS029 | testing.py | 137 |
| M | GS029 | testing.py | 174 |
| M | GS029 | testing.py | 200 |
| M | GS029 | testing.py | 300 |
| M | GS029 | tests.py | 135 |
| M | GS029 | tests.py | 20 |
| M | GS029 | tests.py | 100 |
| M | GS029 | tests.py | 8 |
| M | GS029 | tests.py | 9 |
| M | GS029 | tests.py | 57 |
| M | GS029 | tests.py | 229 |
| M | GS029 | tests.py | 23 |
| M | GS029 | tests.py | 648 |
| M | GS029 | tests.py | 162 |
| M | GS029 | tests.py | 181 |
| M | GS029 | tests.py | 196 |
| M | GS029 | tests.py | 233 |
| M | GS029 | tests.py | 261 |
| M | GS029 | tests.py | 319 |
| M | GS029 | tests.py | 320 |
| M | GS029 | tests.py | 332 |
| M | GS029 | tests.py | 333 |
| M | GS029 | tests.py | 334 |
| M | GS029 | tests.py | 335 |
| M | GS029 | tests.py | 740 |
| M | GS029 | tests.py | 741 |
| M | GS029 | tests.py | 742 |
| M | GS029 | tests.py | 743 |
| M | GS029 | tests.py | 744 |
| M | GS029 | tests.py | 812 |
| M | GS029 | tests.py | 813 |
| M | GS029 | tests.py | 814 |
| M | GS029 | tests.py | 867 |
| M | GS029 | tests.py | 868 |
| M | GS029 | tests.py | 869 |
| M | GS029 | tests.py | 32 |
| M | GS029 | tests.py | 44 |
| M | GS029 | tests.py | 57 |
| M | GS029 | tests.py | 58 |
| M | GS029 | tests.py | 59 |
| M | GS029 | tests.py | 60 |
| M | GS029 | tests.py | 61 |
| M | GS029 | tests.py | 139 |
| M | GS029 | tests.py | 491 |
| M | GS029 | tests.py | 149 |
| M | GS029 | tests.py | 168 |
| M | GS029 | tests.py | 186 |
| M | GS029 | tests.py | 205 |
| M | GS029 | tests.py | 209 |
| M | GS029 | tests.py | 608 |
| M | GS029 | tests.py | 613 |
| M | GS029 | tests.py | 926 |
| M | GS029 | tests.py | 1207 |
| M | GS029 | tests.py | 1317 |
| M | GS029 | tests.py | 1357 |
| M | GS029 | tests.py | 1509 |
| M | GS029 | tests.py | 1673 |
| M | GS029 | tests.py | 1957 |
| M | GS029 | tests.py | 1958 |
| M | GS029 | tests.py | 1977 |
| M | GS029 | tests.py | 50 |
| M | GS029 | tests.py | 296 |
| M | GS029 | tests.py | 41 |
| M | GS029 | tests.py | 366 |
| M | GS029 | tests.py | 114 |
| M | GS029 | tests.py | 133 |
| M | GS029 | tests.py | 151 |
| M | GS029 | tests.py | 242 |
| C | GS001 | generator.py | 12 |
| C | GS001 | tests.py | 114 |
| C | GS001 | tests.py | 133 |
| C | GS001 | tests.py | 151 |
| C | GS001 | tests.py | 242 |
| C | GS001 | tests.py | 319 |
| C | GS001 | testing.py | 137 |
| C | GS001 | app.example.yaml | 20 |
| C | GS001 | config.py | 12 |
| C | GS001 | prod.example.yaml | 20 |
| L | GS003 | tests.py | 360 |
| L | GS003 | tests.py | 632 |
| L | GS003 | tests.py | 268 |
| L | GS003 | tests.py | 193 |
| L | GS003 | tests.py | 228 |
| L | GS003 | tests.py | 265 |
| L | GS003 | generator.py | 103 |
| L | GS003 | generator.py | 126 |
| L | GS003 | tests.py | 352 |
| L | GS003 | tests.py | 143 |
| L | GS003 | tests.py | 155 |
| L | GS003 | tests.py | 535 |
| L | GS003 | tests.py | 572 |
| L | GS003 | tests.py | 1233 |
| L | GS003 | tests.py | 1886 |
| L | GS003 | tests.py | 384 |
| L | GS003 | tests.py | 445 |
| L | GS003 | tests.py | 687 |
| L | GS003 | tests.py | 715 |
| L | GS003 | testing.py | 495 |
| L | GS003 | 111c4f9eab84_add_ai4d_prc_keys.py | 275 |
| L | GS003 | 111c4f9eab84_add_ai4d_prc_keys.py | 283 |
| L | GS003 | 347a14922cff_ai4d_prc_review_form.py | 418 |
| L | GS003 | 347a14922cff_ai4d_prc_review_form.py | 434 |
| L | GS003 | 34a5a1fce672_ai4d_prc_review_updates.py | 475 |
| L | GS003 | 6b64b8037b7b_prc_review_update2.py | 479 |
| L | GS003 | 6b64b8037b7b_prc_review_update2.py | 495 |
| L | GS003 | 6b64b8037b7b_prc_review_update2.py | 1072 |
| L | GS003 | 6b64b8037b7b_prc_review_update2.py | 1263 |
| L | GS003 | 6b64b8037b7b_prc_review_update2.py | 1337 |
| L | GS003 | e1f99a034c22_add_submitted_to_review_response.py | 19 |
| L | GS003 | e1f99a034c22_add_submitted_to_review_response.py | 30 |
| L | GS003 | FormMultiFile.js | 82 |
| L | GS003 | ResponsePage.js | 495 |
| L | GS003 | ResponsePage.js | 674 |
| L | GS003 | createInvitedGuest.js | 10 |
| L | GS003 | GuestRegistrationComponent.js | 486 |
| L | GS003 | ConfirmPasswordResetForm.js | 65 |
| L | GS003 | ReviewForm.js | 249 |
| L | GS003 | ReviewDashboard.js | 146 |
| L | GS003 | serviceWorker.js | 44 |
| L | GS003 | serviceWorker.js | 72 |
| L | GS003 | serviceWorker.js | 85 |
| L | GS003 | serviceWorker.js | 123 |
| L | GS003 | attendance.service.js | 61 |
| L | GS003 | user.service.js | 199 |
| L | GS008 | config.py | 6 |
| L | GS008 | config.py | 12 |
| L | GS008 | config.py | 17 |
| L | GS008 | config.py | 19 |
| L | GS008 | config.py | 39 |
| I | GS015 | routes.py | 1 |
| I | GS015 | main.py | 1 |
| i | GS020 |  | 123 |
| i | GS020 |  | 58 |
| i | GS020 |  | 220 |
| ? | GS034-token_collector | EventStatus.js | 313 |
| ? | GS034-token_collector | AnswerValue.test.js | 8 |
| ? | GS034-token_collector | MultiFileValue.test.js | 6 |
| ? | GS034-token_collector | serviceWorker.js | 26 |
| ? | GS034-token_collector | serviceWorker.js | 35 |
| ? | GS034-token_collector | applicationForm.service.js | 4 |
| ? | GS034-token_collector | attendance.service.js | 4 |
| ? | GS034-token_collector | content.service.js | 2 |
| ? | GS034-token_collector | engagement.service.js | 4 |
| ? | GS034-token_collector | announcement.service.js | 4 |
| ? | GS034-token_collector | checkin.service.js | 4 |
| ? | GS034-token_collector | connection.service.js | 4 |
| ? | GS034-token_collector | discussion.service.js | 4 |
| ? | GS034-token_collector | profile.service.js | 4 |
| ? | GS034-token_collector | programme.service.js | 4 |
| ? | GS034-token_collector | eventStats.service.js | 4 |
| ? | GS034-token_collector | events.service.js | 4 |
| ? | GS034-token_collector | file.service.js | 4 |
| ? | GS034-token_collector | form.service.js | 4 |
| ? | GS034-token_collector | formConfig.service.js | 4 |
| ? | GS034-token_collector | formResponse.service.js | 4 |
| ? | GS034-token_collector | invitedGuests.service.js | 4 |
| ? | GS034-token_collector | invoices.service.js | 4 |
| ? | GS034-token_collector | offer.service.js | 4 |
| ? | GS034-token_collector | organisation.service.js | 3 |
| ? | GS034-token_collector | outcome.service.js | 4 |
| ? | GS034-token_collector | profilelist.service.js | 4 |
| ? | GS034-token_collector | reference.service.js | 4 |
| ? | GS034-token_collector | registration.admin.service.js | 4 |
| ? | GS034-token_collector | registration.service.js | 4 |
| ? | GS034-token_collector | responses.service.js | 4 |
| ? | GS034-token_collector | review.service.js | 4 |
| ? | GS034-token_collector | tags.service.js | 4 |
| ? | GS034-token_collector | translation.service.js | 4 |
| ? | GS034-token_collector | user.service.js | 4 |
| ? | GS034-token_collector | errorHandlerUtility.js | 4 |
| ? | GS034-token_collector | files.js | 9 |
| ? | GS034-token_collector | files.js | 35 |
| ? | GS034-token_collector | push.js | 3 |
| ? | GS034-token_collector | vite.config.mjs | 9 |
| ? | GS034-token_collector | vite.config.mjs | 22 |
| ? | GS036-dangerously_set_html | ReviewAssignmentComponent.js | 220 |
| ? | GS037-hardcoded_password | tests.py | 608 |
| ? | GS037-hardcoded_password | tests.py | 613 |
| ? | GS037-hardcoded_password | tests.py | 1509 |
| ? | GS037-hardcoded_password | tests.py | 1673 |
| ? | GS037-hardcoded_api_key | generator.py | 12 |
| ? | GS037-hardcoded_password | tests.py | 114 |
| ? | GS037-hardcoded_password | tests.py | 133 |
| ? | GS037-hardcoded_password | tests.py | 151 |
| ? | GS037-hardcoded_password | tests.py | 242 |
| ? | GS037-hardcoded_password | tests.py | 47 |
| ? | GS037-hardcoded_password | tests.py | 48 |
| ? | GS037-hardcoded_password | tests.py | 49 |
| ? | GS037-hardcoded_password | tests.py | 50 |
| ? | GS037-hardcoded_password | tests.py | 51 |
| ? | GS037-hardcoded_password | tests.py | 52 |
| ? | GS037-hardcoded_password | tests.py | 53 |
| ? | GS037-hardcoded_password | tests.py | 54 |
| ? | GS037-hardcoded_password | tests.py | 55 |
| ? | GS037-hardcoded_password | tests.py | 56 |
| ? | GS037-high_risk | tests.py | 1 |
| ? | GS037-hardcoded_password | tests.py | 319 |
| ? | GS037-hardcoded_password | tests.py | 332 |
| ? | GS037-hardcoded_password | tests.py | 333 |
| ? | GS037-hardcoded_password | tests.py | 334 |
| ? | GS037-hardcoded_password | tests.py | 335 |
| ? | GS037-hardcoded_password | tests.py | 740 |
| ? | GS037-hardcoded_password | tests.py | 741 |
| ? | GS037-hardcoded_password | tests.py | 742 |
| ? | GS037-hardcoded_password | tests.py | 743 |
| ? | GS037-hardcoded_password | tests.py | 744 |
| ? | GS037-hardcoded_password | tests.py | 812 |
| ? | GS037-hardcoded_password | tests.py | 813 |
| ? | GS037-hardcoded_password | tests.py | 814 |
| ? | GS037-hardcoded_password | tests.py | 867 |
| ? | GS037-hardcoded_password | tests.py | 868 |
| ? | GS037-hardcoded_password | tests.py | 869 |
| ? | GS037-high_risk | tests.py | 1 |
| ? | GS037-hardcoded_password | testing.py | 116 |
| ? | GS037-hardcoded_password | testing.py | 137 |
| ? | GS037-hardcoded_password | testing.py | 300 |
| ? | GS037-hardcoded_api_key | testing.py | 174 |
| C | GS025 | migrate_database.sh | 6 |
| C | GS025 | migrate_database.sh | 6 |
| C | GS029 | 1c3fda18bad6_.py | 410 |
| C | GS029 | c795c179c2b2_.py | 221 |
| C | GS029 | 15d51e2866ce_add_offer_award_email.py | 84 |
| C | GS029 | 6d34d1ab6864_eeml_review_form.py | 180 |
| C | GS029 | 78f4d11203c5_ai4d_more_changes.py | 388 |
| C | GS029 | de12a6f382c1_ai4d_review_form.py | 178 |
| C | GS029 | de12a6f382c1_ai4d_review_form.py | 309 |
| C | GS029 | bda5cebe15fd_indabax_registration.py | 265 |
| C | GS029 | bda5cebe15fd_indabax_registration.py | 671 |
| C | GS029 | 76c9226545bb_update_review_assigned_template.py | 47 |
| C | GS029 | 76c9226545bb_update_review_assigned_template.py | 57 |
| C | GS029 | 76c9226545bb_update_review_assigned_template.py | 83 |
| C | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 717 |
| C | GS029 | 303140b3cefb_ai4d_scholarship_review1.py | 724 |
| C | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 129 |
| C | GS029 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 |
| C | GS029 | e3e47585f336_section_question_key.py | 21 |
| C | GS029 | e3e47585f336_section_question_key.py | 27 |
| C | GS029 | e3e47585f336_section_question_key.py | 28 |
| C | GS029 | e3e47585f336_section_question_key.py | 29 |
| C | GS029 | e3e47585f336_section_question_key.py | 31 |
| C | GS029 | e3e47585f336_section_question_key.py | 32 |
| C | GS029 | 49663ad38428_add_guest_removal_email_template.py | 41 |
| C | GS029 | 613df2d7a759_update_email_template.py | 18 |
| C | GS029 | 613df2d7a759_update_email_template.py | 22 |
| C | GS029 | 964ead196cb9_add_miniconf_url.py | 35 |
| C | GS029 | 1e05a293f402_eeml_registration_form.py | 185 |
| C | GS029 | 1e05a293f402_eeml_registration_form.py | 317 |
| C | GS029 | 2279e1fa2e49_eeml_review_update2.py | 187 |
| C | GS029 | 2279e1fa2e49_eeml_review_update2.py | 239 |
| C | GS029 | 3bc5355f159c_add_org_url_and_event_fields.py | 31 |
| C | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 475 |
| C | GS029 | 10b4b888c16b_ai4d_first_call_updates.py | 496 |
| C | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 279 |
| C | GS029 | 111c4f9eab84_add_ai4d_prc_keys.py | 281 |
| C | GS029 | 3e7bdff8af80_eeml_form_updates.py | 65 |
| C | GS029 | 70b2a4f4a596_offer_paid_email.py | 71 |
| C | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 24 |
| C | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 25 |
| C | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 26 |
| C | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 27 |
| C | GS029 | fc82c8e54fd7_emailtemplate_language_subject.py | 28 |
| C | GS029 | tests.py | 33 |
| C | GS029 | tests.py | 31 |
| C | GS029 | tests.py | 52 |
| C | GS029 | tests.py | 63 |
| C | GS029 | tests.py | 25 |
| C | GS029 | tests.py | 497 |
| C | GS029 | tests.py | 1287 |
| C | GS029 | tests.py | 1291 |
| C | GS029 | tests.py | 1763 |
| C | GS029 | tests.py | 1772 |
| C | GS029 | tests.py | 2001 |
| C | GS029 | tests.py | 2010 |
| C | GS029 | tests.py | 2219 |
| C | GS029 | tests.py | 38 |
| C | GS029 | tests.py | 396 |
| C | GS029 | tests.py | 540 |
| C | GS029 | tests.py | 636 |
| C | GS029 | tests.py | 677 |
| C | GS029 | tests.py | 20 |
| C | GS029 | tests.py | 100 |
| C | GS029 | tests.py | 57 |
| C | GS029 | tests.py | 229 |
| C | GS029 | tests.py | 23 |
| C | GS029 | tests.py | 648 |
| C | GS029 | tests.py | 320 |
| C | GS029 | tests.py | 32 |
| C | GS029 | tests.py | 44 |
| C | GS029 | tests.py | 57 |
| C | GS029 | tests.py | 58 |
| C | GS029 | tests.py | 59 |
| C | GS029 | tests.py | 60 |
| C | GS029 | tests.py | 61 |
| C | GS029 | tests.py | 926 |
| C | GS029 | tests.py | 1357 |
| C | GS029 | tests.py | 1957 |
| C | GS029 | tests.py | 1958 |
| C | GS029 | tests.py | 1977 |
| C | GS029 | tests.py | 41 |
| C | GS029 | AttendanceTable.js | 525 |
| C | GS029 | TagConfigComponent.js | 230 |
| C | GS029 | TagConfigComponent.js | 300 |
| C | GS029 | TagConfigComponent.js | 379 |
| C | GS029 | TagConfigComponent.js | 380 |
| C | GS029 | InvitedGuestComponent.js | 468 |
| C | GS029 | ResponseListComponent.js | 271 |
| C | GS029 | OfferAdminComponent.js | 403 |
| C | GS029 | ReferenceComponent.js | 117 |
| C | GS029 | InvoiceAdminListComponent.js | 243 |
| C | GS029 | InvoiceAdminListComponent.js | 254 |
| H | GS025 | package-lock.json | 0 |
| H | GS025 | docker-compose.yml | 0 |
| H | GS002 | nginx.conf | 0 |
| C | GS005 | 02242641e122_add_local_event.py | 190 |
| C | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 186 |
| C | GS005 | 0edb89e87e72_indabaxza_offer_email_templates.py | 187 |
| C | GS005 | 1349a2c924f4_.py | 282 |
| C | GS005 | 1c3fda18bad6_.py | 405 |
| C | GS005 | 1e05a293f402_eeml_registration_form.py | 320 |
| C | GS005 | 1e05a293f402_eeml_registration_form.py | 321 |
| C | GS005 | 1e05a293f402_eeml_registration_form.py | 322 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 53 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 53 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 393 |
| C | GS005 | 2241922a3305_redo_french_email_templates.py | 393 |
| C | GS005 | 3ab678fc66cd_populate_reg_form.py | 435 |
| C | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 340 |
| C | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 347 |
| C | GS005 | 4b5d67699684_ai4d_scholarship_call_updates.py | 354 |
| C | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 |
| C | GS005 | 4b881c1c6dc2_add_email_templates.py | 288 |
| C | GS005 | 62c7711123a8_french_email_templates.py | 367 |
| C | GS005 | 62c7711123a8_french_email_templates.py | 367 |
| C | GS005 | 964ead196cb9_add_miniconf_url.py | 36 |
| C | GS005 | bda5cebe15fd_indabax_registration.py | 674 |
| C | GS005 | bda5cebe15fd_indabax_registration.py | 675 |
| C | GS005 | bda5cebe15fd_indabax_registration.py | 676 |
| C | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 |
| C | GS005 | cebfdfef31cd_assign_action_editor_email_template.py | 69 |
| I | GS007 | 0023aeda53b0_.py | 25 |
| I | GS007 | 21018201594d_offer_event_fee.py | 27 |
| I | GS007 | 36235e184d09_.py | 28 |
| I | GS007 | 36235e184d09_.py | 29 |
| I | GS007 | 36235e184d09_.py | 30 |
| I | GS007 | 36235e184d09_.py | 31 |
| I | GS007 | 3e271c360a92_remove_offer_awards.py | 28 |
| I | GS007 | 3e271c360a92_remove_offer_awards.py | 29 |
| I | GS007 | 3e271c360a92_remove_offer_awards.py | 30 |
| I | GS007 | 3e271c360a92_remove_offer_awards.py | 31 |
| I | GS007 | 44df297ad858_.py | 26 |
| I | GS007 | 44df297ad858_.py | 27 |
| I | GS007 | 627a96dad7e8_registration_section_show_for_tags.py | 29 |
| I | GS007 | 627a96dad7e8_registration_section_show_for_tags.py | 30 |
| I | GS007 | 627a96dad7e8_registration_section_show_for_tags.py | 31 |
| I | GS007 | 8a1468838847_.py | 28 |
| I | GS007 | 91468f804113_.py | 25 |
| I | GS007 | b6a2a69fbb13_.py | 28 |
| I | GS007 | c06c236ad4c5_.py | 29 |
| I | GS007 | c06c236ad4c5_.py | 30 |
| I | GS007 | c06c236ad4c5_.py | 31 |
| I | GS007 | c0885e531d29_.py | 41 |
| I | GS007 | c0885e531d29_.py | 42 |
| I | GS007 | c0885e531d29_.py | 43 |
| s | GS009 |  | 0 |
| H | GS011 | testing.py | 174 |
| L | GS012 | api.py | 235 |
| L | GS012 | api.py | 178 |
| L | GS012 | api.py | 230 |
| L | GS012 | api.py | 286 |
| L | GS012 | api.py | 528 |
| L | GS012 | tests.py | 155 |
| L | GS012 | tests.py | 330 |
| L | GS012 | tests.py | 355 |
| L | GS012 | api.py | 803 |
| L | GS012 | api.py | 823 |
| L | GS012 | api.py | 861 |
| L | GS012 | api.py | 223 |
| L | GS012 | api.py | 230 |
| L | GS012 | api.py | 255 |
| L | GS012 | api.py | 318 |
| L | GS012 | api.py | 371 |
| L | GS012 | api.py | 381 |
| L | GS012 | tests.py | 138 |
| L | GS012 | api.py | 68 |
| H | GS014 | config.py | 12 |
| C | GS016 | migrate_database.sh | 6 |
| C | GS016 | migrate_database.sh | 6 |
| H | GS017 | api.py | 221 |
| H | GS017 | api.py | 265 |
| H | GS017 | util.js | 700 |
| H | GS017 | DiscussionSpaces.js | 175 |
| H | GS018 | api.py | 268 |
| M | GS019 | models.py | 64 |
| C | GS019 | testing.py | 174 |
| s | GS021 |  | 22 |
| s | GS021 |  | 266 |
| s | GS021 |  | 352 |
| s | GS021 |  | 49 |
| s | GS021 |  | 24 |
| s | GS021 |  | 34 |
| s | GS021 |  | 13 |
| s | GS021 |  | 14 |
| s | GS021 |  | 37 |
| r | GS022 |  | 131 |
| r | GS022 |  | 133 |
| r | GS022 |  | 331 |
| r | GS022 |  | 26 |
| r | GS022 |  | 88 |
| r | GS022 |  | 30 |
| r | GS022 |  | 333 |
| r | GS022 |  | 356 |
| r | GS022 |  | 18 |
| r | GS022 |  | 111 |
| r | GS022 |  | 8 |
| r | GS022 |  | 34 |
| r | GS022 |  | 54 |
| r | GS022 |  | 10 |
| r | GS022 |  | 39 |
| r | GS022 |  | 71 |
| r | GS022 |  | 135 |
| r | GS022 |  | 10 |
| r | GS022 |  | 57 |
| r | GS022 |  | 140 |
| r | GS022 |  | 145 |
| r | GS022 |  | 416 |
| r | GS022 |  | 423 |
| r | GS022 |  | 12 |
| r | GS022 |  | 171 |
| r | GS022 |  | 109 |
| r | GS022 |  | 124 |
| r | GS022 |  | 184 |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-eval_usage |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| ? | GS025-hardcoded_secret |  | ? |
| H | ? | sw.js | 46 |

---
*Сгенерировано GSC v0.6 · 2026-08-09T12:01:37.797398*
# Densory Tickets — Konfiguration

Die folgenden Einstellungen stehen für dieses Produkt zur Verfügung:

Alle folgenden Einstellungen konfigurierst du in deinem [Control Center](https://densory.com/dashboard).

| Key | Typ | Default | Beschreibung |
| --- | --- | --- | --- |
| `locale` | `string` | `""` | Sprache |
| `default_color` | `hexColor` | `#444444` | Standardfarbe |
| `success_color` | `hexColor` | `#2bfc71` | Erfolgsfarbe |
| `warning_color` | `hexColor` | `#ffd621` | Warnfarbe |
| `error_color` | `hexColor` | `#fc251e` | Fehlerfarbe |
| `success_img` | `image` | `/uploads/assets/product-images/discord-bots/default/success.png` | Erfolgsbild |
| `warning_img` | `image` | `/uploads/assets/product-images/discord-bots/default/warning.png` | Warnbild |
| `error_img` | `image` | `/uploads/assets/product-images/discord-bots/default/error.png` | Fehlerbild |
| `tickets_status` | `string` | `enabled` | Ticketsystem |
| `role_hierarchy` | `hierarchy` | `[]` | Rollen-Hierarchie |
| `tickets_staff_min_group` | `group_select` | `2` | Team ab Gruppe |
| `tickets_lead_min_group` | `group_select` | `1` | Leitung ab Gruppe |
| `tickets_admin_min_group` | `group_select` | `0` | Verwaltung ab Gruppe |
| `tickets_staff_roles` | `roles` | `[]` | Team-Rollen |
| `tickets_lead_roles` | `roles` | `[]` | Leitungs-Rollen |
| `tickets_log_channel` | `channel` | `""` | Log-Kanal |
| `ticket_language_mode` | `string` | `auto` | Sprachwahl |
| `ticket_language_offer` | `array` | `["de","en"]` | Angebotene Sprachen |
| `ticket_language_roles` | `object` | `{}` | Sprache je Rolle |
| `panel_locale_mode` | `string` | `guild` | Sprache des Panels |
| `ui_style` | `string` | `v2` | Kartendarstellung |
| `ticket_categories` | `object` | `{"version":2,"defaults":{"container_kind":"channel","name_template":"{icon}{number}-{user}","waiting_name_template":"neu-{number}","slowmode_seconds":5,"max_open_per_user":1,"cooldown_seconds":60,"ask_feedback":true,"dm_transcript":true},"categories":[{"key":"support","sort":0,"mode":"support","name":{"de":"Support","en":"Support"},"description":{"de":"Frage stellen oder Problem melden","en":"Ask a question or report a problem"},"icon":"icon_cat_support","color":"#5865F2","questions":[{"id":"topic","type":"select","required":true,"label":{"de":"Worum geht es?","en":"What is this about?"},"options":[{"value":"tech","label":{"de":"Technisches Problem","en":"Technical problem"}},{"value":"account","label":{"de":"Konto oder Zugang","en":"Account or access"}},{"value":"other","label":{"de":"Etwas anderes","en":"Something else"}}]},{"id":"subject","type":"short","group":"main","required":true,"max":80,"label":{"de":"Betreff","en":"Subject"}},{"id":"desc","type":"paragraph","group":"main","required":true,"min":10,"max":1500,"label":{"de":"Beschreibung","en":"Description"},"help":{"de":"Was hast du versucht und was ist passiert?","en":"What did you try and what happened?"},"ai_hint":"Kern des Problems"},{"id":"steps","type":"paragraph","group":"main","required":false,"max":1000,"when":{"all":[{"q":"topic","op":"eq","value":"tech"}]},"label":{"de":"Schritte zum Nachstellen","en":"Steps to reproduce"}}],"on_submit":{"priority":"normal"},"on_close":{"ask_feedback":true,"dm_transcript":true}},{"key":"apply","sort":1,"mode":"application","name":{"de":"Bewerbung","en":"Application"},"description":{"de":"Bewirb dich für das Team","en":"Apply to join the team"},"icon":"icon_cat_application","color":"#10b981","access":{"cooldown_seconds":300,"min_account_age_days":7},"questions":[{"id":"name","type":"short","group":"you","required":true,"max":40,"label":{"de":"Wie sollen wir dich nennen?","en":"What should we call you?"}},{"id":"age","type":"number","group":"you","required":true,"integer":true,"min":13,"max":99,"label":{"de":"Wie alt bist du?","en":"How old are you?"}},{"id":"hours","type":"select","group":"you","required":true,"label":{"de":"Zeit pro Woche","en":"Time per week"},"options":[{"value":"lt5","label":{"de":"unter 5 Stunden","en":"under 5 hours"}},{"value":"5_10","label":{"de":"5 bis 10 Stunden","en":"5 to 10 hours"}},{"value":"gt10","label":{"de":"mehr als 10 Stunden","en":"more than 10 hours"}}]},{"id":"experience","type":"yesno","required":true,"label":{"de":"Hast du schon in einem Team gearbeitet?","en":"Have you worked in a team before?"},"yes_label":{"de":"Ja","en":"Yes"},"no_label":{"de":"Nein","en":"No"}},{"id":"exp_detail","type":"paragraph","group":"story","required":true,"min":20,"max":1000,"when":{"all":[{"q":"experience","op":"is_true"}]},"label":{"de":"Wo und wie lange?","en":"Where and for how long?"}},{"id":"motivation","type":"paragraph","group":"story","required":true,"min":30,"max":1500,"label":{"de":"Warum möchtest du ins Team?","en":"Why do you want to join the team?"},"ai_hint":"Motivation der Bewerbung"}],"on_submit":{"priority":"normal","welcome":{"de":"Danke für deine Bewerbung! Wir melden uns.","en":"Thanks for your application! We will get back to you."}},"on_close":{"ask_feedback":false,"dm_transcript":true}}]}` | Kategorien & Fragen |
| `ticket_quiz_pools` | `object` | `{}` | Fragenpools für Tests |
| `panel_layout` | `string` | `select` | Aufbau |
| `panel_accent_color` | `hexColor` | `#5865F2` | Akzentfarbe |
| `panel_title` | `string` | `""` | Überschrift |
| `panel_text` | `string` | `""` | Text |
| `panel_show_eta` | `string` | `enabled` | Antwortzeit zeigen |
| `panel_show_open_count` | `string` | `disabled` | Offene Tickets zeigen |
| `panel_cooldown_seconds` | `number` | `10` | Sperre nach Klick (Sekunden) |
| `ticket_parent_category` | `channel` | `""` | Kategorie für Tickets |
| `ticket_waiting_category` | `channel` | `""` | Kategorie für Fragen |
| `ticket_archive_category` | `channel` | `""` | Archiv-Kategorie |
| `ticket_name_template` | `string` | `{icon}{number}-{user}` | Namensschablone |
| `ticket_waiting_name_template` | `string` | `neu-{number}` | Namensschablone während der Fragen |
| `ticket_number_start` | `number` | `1` | Erste Ticketnummer |
| `ticket_slowmode_seconds` | `number` | `5` | Langsamer Modus (Sekunden) |
| `ticket_max_open_per_user` | `number` | `1` | Offene Tickets je Person |
| `ticket_max_open_total` | `number` | `0` | Offene Tickets insgesamt |
| `ticket_rate_per_hour` | `number` | `3` | Tickets je Stunde und Person |
| `ticket_show_progress` | `string` | `enabled` | Fortschritt zeigen |
| `ticket_allow_back` | `string` | `enabled` | Zurückgehen erlauben |
| `ticket_review_step` | `string` | `enabled` | Zusammenfassung vor dem Absenden |
| `claim_enabled` | `string` | `enabled` | Übernehmen erlauben |
| `claim_exclusive` | `string` | `disabled` | Nur die übernehmende Person |
| `claim_release_min_group` | `group_select` | `1` | Fremde Übernahme lösen ab Gruppe |
| `ping_roles_on_submit` | `roles` | `[]` | Rollen benachrichtigen |
| `ping_style` | `string` | `mention` | Art der Benachrichtigung |
| `staff_note_enabled` | `string` | `enabled` | Interne Notizen |
| `close_min_group` | `group_select` | `2` | Schließen ab Gruppe |
| `close_by_opener` | `string` | `enabled` | Ersteller darf schließen |
| `close_require_reason` | `string` | `enabled` | Grund verlangen |
| `close_delay_seconds` | `number` | `10` | Wartezeit vor dem Löschen (Sekunden) |
| `close_action` | `string` | `delete` | Was beim Schließen passiert |
| `transcript_enabled` | `string` | `enabled` | Protokoll erstellen |
| `transcript_format` | `string` | `html` | Format des Protokolls |
| `transcript_dm_opener` | `string` | `enabled` | Protokoll an den Ersteller |
| `transcript_channel` | `channel` | `""` | Kanal für Protokolle |
| `transcript_max_messages` | `number` | `2000` | Nachrichten je Protokoll |
| `feedback_enabled` | `string` | `enabled` | Nach Bewertung fragen |
| `feedback_channel_mode` | `string` | `dm` | Wo gefragt wird |
| `feedback_ask_reason` | `string` | `enabled` | Bei schlechter Bewertung nachfragen |
| `feedback_log_channel` | `channel` | `""` | Kanal für Bewertungen |
| `automation_enabled` | `string` | `enabled` | Automatik |
| `abandon_after_minutes` | `number` | `60` | Abbruch nach (Minuten) |
| `inactivity_hours` | `number` | `48` | Stille bis zum Schließen (Stunden) |
| `inactivity_warn_hours` | `number` | `24` | Vorwarnung nach (Stunden) |
| `inactivity_scope` | `string` | `unanswered_by_user` | Was als Stille zählt |
| `alert_default_hours` | `number` | `24` | Voreinstellung für Erinnerungen (Stunden) |
| `auto_priority_by_age_hours` | `number` | `0` | Priorität nach Alter anheben (Stunden) |
| `icon_panel_img` | `image` | `""` | Panel |
| `icon_ticket_img` | `image` | `""` | Ticket-Deckblatt |
| `icon_step_img` | `image` | `""` | Frage |
| `icon_summary_img` | `image` | `""` | Zusammenfassung |
| `icon_wait_img` | `image` | `""` | Arbeitskarte |
| `icon_claim_img` | `image` | `""` | Übernehmen |
| `icon_close_img` | `image` | `""` | Schließen |
| `icon_user_img` | `image` | `""` | Nutzer |
| `icon_more_img` | `image` | `""` | Mehr-Menü |
| `icon_lock_img` | `image` | `""` | Sperren |
| `icon_transcript_img` | `image` | `""` | Protokoll |
| `icon_feedback_img` | `image` | `""` | Bewertung |
| `icon_alert_img` | `image` | `""` | Erinnerung |
| `icon_ai_img` | `image` | `""` | KI-Hilfe |
| `icon_quiz_img` | `image` | `""` | Test |
| `icon_cat_support_img` | `image` | `""` | Kategorie: Support |
| `icon_cat_application_img` | `image` | `""` | Kategorie: Bewerbung |
| `icon_cat_report_img` | `image` | `""` | Kategorie: Meldung |
| `icon_cat_order_img` | `image` | `""` | Kategorie: Bestellung |
| `icon_cat_custom_img` | `image` | `""` | Kategorie: Sonstiges |
| `ai_enabled` | `string` | `disabled` | KI-Hilfen |
| `ai_summary_enabled` | `string` | `disabled` | Zusammenfassung |
| `ai_summary_on_close` | `string` | `disabled` | Zusammenfassung beim Schließen |
| `ai_reply_enabled` | `string` | `disabled` | Antwortvorschlag |
| `ai_translate_enabled` | `string` | `disabled` | Übersetzung |
| `ai_triage_enabled` | `string` | `disabled` | Priorität vorschlagen |
| `ai_reply_style` | `string` | `friendly` | Tonfall der Vorschläge |
| `ai_context_messages` | `number` | `40` | Nachrichten als Kontext |
| `ai_triage_min_confidence` | `number` | `70` | Mindestsicherheit für Vorschläge (%) |
| `ai_min_group` | `group_select` | `2` | KI nutzen ab Gruppe |
| `ai_notice_in_ticket` | `string` | `enabled` | Hinweis im Ticket |
| `retention_days` | `number` | `90` | Tickets aufbewahren (Tage) |
| `retention_application_days` | `number` | `180` | Bewerbungstests aufbewahren (Tage) |
| `retention_feedback_days` | `number` | `365` | Bewertungen aufbewahren (Tage) |
| `transcript_retention_days` | `number` | `180` | Protokolle aufbewahren (Tage) |
| `stats_retention_days` | `number` | `730` | Statistik aufbewahren (Tage) |
| `privacy_admin_min_group` | `group_select` | `0` | Datenschutz-Befehle ab Gruppe |
| `report_visibility` | `string` | `leads` | Wer Meldungen sieht |
| `privacy_notice_text` | `string` | `""` | Eigener Datenschutzhinweis |

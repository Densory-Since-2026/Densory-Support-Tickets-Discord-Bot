# Densory Tickets — Configuration

The following settings are available for this product:

All settings below are configured in your [Control Center](https://densory.com/dashboard).

| Key | Type | Default | Description |
| --- | --- | --- | --- |
| `locale` | `string` | `""` | Locale |
| `default_color` | `hexColor` | `#444444` | Default color |
| `success_color` | `hexColor` | `#2bfc71` | Success color |
| `warning_color` | `hexColor` | `#ffd621` | Warning color |
| `error_color` | `hexColor` | `#fc251e` | Error color |
| `success_img` | `image` | `/uploads/assets/product-images/discord-bots/default/success.png` | Success image |
| `warning_img` | `image` | `/uploads/assets/product-images/discord-bots/default/warning.png` | Warning image |
| `error_img` | `image` | `/uploads/assets/product-images/discord-bots/default/error.png` | Error image |
| `tickets_status` | `string` | `enabled` | Ticket system |
| `role_hierarchy` | `hierarchy` | `[]` | Role hierarchy |
| `tickets_staff_min_group` | `group_select` | `2` | Team from group |
| `tickets_lead_min_group` | `group_select` | `1` | Leads from group |
| `tickets_admin_min_group` | `group_select` | `0` | Administration from group |
| `tickets_staff_roles` | `roles` | `[]` | Team roles |
| `tickets_lead_roles` | `roles` | `[]` | Lead roles |
| `tickets_log_channel` | `channel` | `""` | Log channel |
| `ticket_language_mode` | `string` | `auto` | Language choice |
| `ticket_language_offer` | `array` | `["de","en"]` | Offered languages |
| `ticket_language_roles` | `object` | `{}` | Language per role |
| `panel_locale_mode` | `string` | `guild` | Panel language |
| `ui_style` | `string` | `v2` | Card style |
| `ticket_categories` | `object` | `{"version":2,"defaults":{"container_kind":"channel","name_template":"{icon}{number}-{user}","waiting_name_template":"neu-{number}","slowmode_seconds":5,"max_open_per_user":1,"cooldown_seconds":60,"ask_feedback":true,"dm_transcript":true},"categories":[{"key":"support","sort":0,"mode":"support","name":{"de":"Support","en":"Support"},"description":{"de":"Frage stellen oder Problem melden","en":"Ask a question or report a problem"},"icon":"icon_cat_support","color":"#5865F2","questions":[{"id":"topic","type":"select","required":true,"label":{"de":"Worum geht es?","en":"What is this about?"},"options":[{"value":"tech","label":{"de":"Technisches Problem","en":"Technical problem"}},{"value":"account","label":{"de":"Konto oder Zugang","en":"Account or access"}},{"value":"other","label":{"de":"Etwas anderes","en":"Something else"}}]},{"id":"subject","type":"short","group":"main","required":true,"max":80,"label":{"de":"Betreff","en":"Subject"}},{"id":"desc","type":"paragraph","group":"main","required":true,"min":10,"max":1500,"label":{"de":"Beschreibung","en":"Description"},"help":{"de":"Was hast du versucht und was ist passiert?","en":"What did you try and what happened?"},"ai_hint":"Kern des Problems"},{"id":"steps","type":"paragraph","group":"main","required":false,"max":1000,"when":{"all":[{"q":"topic","op":"eq","value":"tech"}]},"label":{"de":"Schritte zum Nachstellen","en":"Steps to reproduce"}}],"on_submit":{"priority":"normal"},"on_close":{"ask_feedback":true,"dm_transcript":true}},{"key":"apply","sort":1,"mode":"application","name":{"de":"Bewerbung","en":"Application"},"description":{"de":"Bewirb dich für das Team","en":"Apply to join the team"},"icon":"icon_cat_application","color":"#10b981","access":{"cooldown_seconds":300,"min_account_age_days":7},"questions":[{"id":"name","type":"short","group":"you","required":true,"max":40,"label":{"de":"Wie sollen wir dich nennen?","en":"What should we call you?"}},{"id":"age","type":"number","group":"you","required":true,"integer":true,"min":13,"max":99,"label":{"de":"Wie alt bist du?","en":"How old are you?"}},{"id":"hours","type":"select","group":"you","required":true,"label":{"de":"Zeit pro Woche","en":"Time per week"},"options":[{"value":"lt5","label":{"de":"unter 5 Stunden","en":"under 5 hours"}},{"value":"5_10","label":{"de":"5 bis 10 Stunden","en":"5 to 10 hours"}},{"value":"gt10","label":{"de":"mehr als 10 Stunden","en":"more than 10 hours"}}]},{"id":"experience","type":"yesno","required":true,"label":{"de":"Hast du schon in einem Team gearbeitet?","en":"Have you worked in a team before?"},"yes_label":{"de":"Ja","en":"Yes"},"no_label":{"de":"Nein","en":"No"}},{"id":"exp_detail","type":"paragraph","group":"story","required":true,"min":20,"max":1000,"when":{"all":[{"q":"experience","op":"is_true"}]},"label":{"de":"Wo und wie lange?","en":"Where and for how long?"}},{"id":"motivation","type":"paragraph","group":"story","required":true,"min":30,"max":1500,"label":{"de":"Warum möchtest du ins Team?","en":"Why do you want to join the team?"},"ai_hint":"Motivation der Bewerbung"}],"on_submit":{"priority":"normal","welcome":{"de":"Danke für deine Bewerbung! Wir melden uns.","en":"Thanks for your application! We will get back to you."}},"on_close":{"ask_feedback":false,"dm_transcript":true}}]}` | Categories & questions |
| `ticket_quiz_pools` | `object` | `{}` | Question pools for tests |
| `panel_layout` | `string` | `select` | Layout |
| `panel_accent_color` | `hexColor` | `#5865F2` | Accent colour |
| `panel_title` | `string` | `""` | Headline |
| `panel_text` | `string` | `""` | Text |
| `panel_show_eta` | `string` | `enabled` | Show response time |
| `panel_show_open_count` | `string` | `disabled` | Show open tickets |
| `panel_cooldown_seconds` | `number` | `10` | Cooldown after a click (seconds) |
| `ticket_parent_category` | `channel` | `""` | Category for tickets |
| `ticket_waiting_category` | `channel` | `""` | Category for questions |
| `ticket_archive_category` | `channel` | `""` | Archive category |
| `ticket_name_template` | `string` | `{icon}{number}-{user}` | Name template |
| `ticket_waiting_name_template` | `string` | `neu-{number}` | Name template during the questions |
| `ticket_number_start` | `number` | `1` | First ticket number |
| `ticket_slowmode_seconds` | `number` | `5` | Slow mode (seconds) |
| `ticket_max_open_per_user` | `number` | `1` | Open tickets per person |
| `ticket_max_open_total` | `number` | `0` | Open tickets in total |
| `ticket_rate_per_hour` | `number` | `3` | Tickets per hour and person |
| `ticket_show_progress` | `string` | `enabled` | Show progress |
| `ticket_allow_back` | `string` | `enabled` | Allow going back |
| `ticket_review_step` | `string` | `enabled` | Summary before submitting |
| `claim_enabled` | `string` | `enabled` | Allow claiming |
| `claim_exclusive` | `string` | `disabled` | Only the person who claimed |
| `claim_release_min_group` | `group_select` | `1` | Release a foreign claim from group |
| `ping_roles_on_submit` | `roles` | `[]` | Roles to notify |
| `ping_style` | `string` | `mention` | Kind of notification |
| `staff_note_enabled` | `string` | `enabled` | Internal notes |
| `close_min_group` | `group_select` | `2` | Closing from group |
| `close_by_opener` | `string` | `enabled` | The opener may close |
| `close_require_reason` | `string` | `enabled` | Require a reason |
| `close_delay_seconds` | `number` | `10` | Delay before deleting (seconds) |
| `close_action` | `string` | `delete` | What happens on close |
| `transcript_enabled` | `string` | `enabled` | Build a transcript |
| `transcript_format` | `string` | `html` | Transcript format |
| `transcript_dm_opener` | `string` | `enabled` | Transcript to the opener |
| `transcript_channel` | `channel` | `""` | Channel for transcripts |
| `transcript_max_messages` | `number` | `2000` | Messages per transcript |
| `feedback_enabled` | `string` | `enabled` | Ask for a rating |
| `feedback_channel_mode` | `string` | `dm` | Where to ask |
| `feedback_ask_reason` | `string` | `enabled` | Ask again on a poor rating |
| `feedback_log_channel` | `channel` | `""` | Channel for ratings |
| `automation_enabled` | `string` | `enabled` | Automation |
| `abandon_after_minutes` | `number` | `60` | Abandon after (minutes) |
| `inactivity_hours` | `number` | `48` | Silence until closing (hours) |
| `inactivity_warn_hours` | `number` | `24` | Warning after (hours) |
| `inactivity_scope` | `string` | `unanswered_by_user` | What counts as silence |
| `alert_default_hours` | `number` | `24` | Default for reminders (hours) |
| `auto_priority_by_age_hours` | `number` | `0` | Raise priority by age (hours) |
| `icon_panel_img` | `image` | `""` | Panel |
| `icon_ticket_img` | `image` | `""` | Ticket cover |
| `icon_step_img` | `image` | `""` | Question |
| `icon_summary_img` | `image` | `""` | Summary |
| `icon_wait_img` | `image` | `""` | Working card |
| `icon_claim_img` | `image` | `""` | Claim |
| `icon_close_img` | `image` | `""` | Close |
| `icon_user_img` | `image` | `""` | Members |
| `icon_more_img` | `image` | `""` | More menu |
| `icon_lock_img` | `image` | `""` | Lock |
| `icon_transcript_img` | `image` | `""` | Transcript |
| `icon_feedback_img` | `image` | `""` | Rating |
| `icon_alert_img` | `image` | `""` | Reminder |
| `icon_ai_img` | `image` | `""` | AI assistance |
| `icon_quiz_img` | `image` | `""` | Test |
| `icon_cat_support_img` | `image` | `""` | Category: support |
| `icon_cat_application_img` | `image` | `""` | Category: application |
| `icon_cat_report_img` | `image` | `""` | Category: report |
| `icon_cat_order_img` | `image` | `""` | Category: order |
| `icon_cat_custom_img` | `image` | `""` | Category: other |
| `ai_enabled` | `string` | `disabled` | AI assistance |
| `ai_summary_enabled` | `string` | `disabled` | Summary |
| `ai_summary_on_close` | `string` | `disabled` | Summary when closing |
| `ai_reply_enabled` | `string` | `disabled` | Draft reply |
| `ai_translate_enabled` | `string` | `disabled` | Translation |
| `ai_triage_enabled` | `string` | `disabled` | Suggest a priority |
| `ai_reply_style` | `string` | `friendly` | Tone of the drafts |
| `ai_context_messages` | `number` | `40` | Messages used as context |
| `ai_triage_min_confidence` | `number` | `70` | Minimum confidence for suggestions (%) |
| `ai_min_group` | `group_select` | `2` | Use AI from group |
| `ai_notice_in_ticket` | `string` | `enabled` | Notice inside the ticket |
| `retention_days` | `number` | `90` | Keep tickets (days) |
| `retention_application_days` | `number` | `180` | Keep application tests (days) |
| `retention_feedback_days` | `number` | `365` | Keep ratings (days) |
| `transcript_retention_days` | `number` | `180` | Keep transcripts (days) |
| `stats_retention_days` | `number` | `730` | Keep statistics (days) |
| `privacy_admin_min_group` | `group_select` | `0` | Privacy commands from group |
| `report_visibility` | `string` | `leads` | Who sees reports |
| `privacy_notice_text` | `string` | `""` | Your own privacy notice |

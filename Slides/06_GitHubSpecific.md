# Github-Spezifisches

## Fokus Github als Projektmanagement-Tool

- Issues (& Pull-Requests)
   - Ähnlich zu Tickets (siehe JIRA, Forenthreads o.ä.)
   - Haben Attribute (z.B. `status`, `assignee`, `due-date`)
- Labels: Spezielles Attribut (von Issues). Nicht zu verwechseln mit Tags (das sind Labels von spezifischen Commits)
- Assignees: Spezielles Attribut (von Issues)
- Projects
   - Hat mehrere konfigurierbare Views (Ansichten)
   - Muss aktiv Issues zu Projekt hinzufügen, damit diese in Ansichten angezeigt werden können
- Milestones: Weitere "Box", um Issues zu gruppieren.

## HOWTO projectmanagement: quick and minimalistic

- Man benötigt eine Liste, in der TODO-Items/Tasks gesammelt werden
- Man braucht eine Ansicht, welche Items einer Person zugewiesen sind
- Man brauch eine Ansicht im Projekt, um planen zu können
    - Kann beliebig weiter ergänzt werden, je nach Bedarf
    - KEEP IT SIMPLE!

### Lösungsvorschlag

- In GitHub ein Projekt erstellen
- Einfaches Board anlegen
- Alle Issues dem Board hinzufügen bzw.direkt dort erstellen
- Allen Issues Assignees geben
- Feld Status (`todo`, `progress`, `done`) für Tracking verwenden

## Best Practices

- Keep it simple, stupid! (KISS)
   - Don't create complexity if you don't need it!
   - Lower maintenance effort
   - Shorter onboarding time
- Show, don't tell.
- If needed, create examples and a HOWTO.
- Differentiate between planning and doing
    - For doing: every person has 1 view for all their tasks
    - For planning: should be different view than the doing-view. Keep it simple! *evtl. comic (Krieg und Freitag, wie, wenn man geplant hat, ist noch nichts gemacht?!)*
- Learn the concept, not the tools!
- Make every item (task, project, etc.) self-explanatory!
   - Explicit, not implicit.
   - No hidden knowledge.
   - Exception: if the item is created and filled live by everyone who works on it, and all questions are answered. Then you can be implicit

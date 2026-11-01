# Tadween sync setup

Current section: cross-device sync. The app code supports one account on iPhone and Windows, deadline sync, and private document storage. The live app needs a Supabase project configured.

1. Create a Supabase project at https://supabase.com/dashboard.
2. Open SQL Editor and run the exact contents of `supabase.sql`.
3. In Authentication → Providers, enable Email. Confirm your email address when registering.
4. Copy Project URL and the publishable/anon key from Project Settings → API into `sync-config.js`. Never put the service_role key there.
5. Commit `sync-config.js` to main. GitHub Pages deploys automatically. Sign in with the same email and password on both devices.
6. Upload PDFs or .docx files from the laptop. They appear in Your documents on the iPhone; tap a filename to view or download it.

Limits: scanned PDFs still require OCR; dates extracted from text need review. Documents uploaded before sign-in were not stored online and must be uploaded again. The 20 MB per-file limit applies. Local browser data remains until its owner signs in; existing dates then sync. The Supabase project may have costs or quotas depending on usage and plan.

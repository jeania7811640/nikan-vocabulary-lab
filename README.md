日韓單字 Lab - Supabase connected frontend

1. Supabase Dashboard -> SQL Editor, paste and run schema.sql.
2. Authentication -> Providers: ensure Email provider is enabled.
3. Authentication -> URL Configuration: add your Vercel URL to allowed redirect URLs.
4. Replace index.html in your GitHub repository root with this index.html and commit. Vercel should redeploy.
5. Open the Vercel URL, create an account, verify email if requested, then sign in.
6. Confirm the sync status. Export CSV before testing as a backup.

Security: the HTML includes only the public publishable key. Never put a secret/service_role key in browser code. RLS policies restrict records to the signed-in user.
Limitations: initial sync merges by Chinese/Japanese/Korean term. Deletion propagation and robust concurrent edit conflict resolution are not yet implemented.

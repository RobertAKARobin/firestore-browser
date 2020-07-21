# Firestore Browser

1. Put your Firebase creds in files named `env.{environment_name}.json`, e.g. `env.dev.json`.
2. Go to `/?env={environment_name}&path={firestore_path}`, e.g. `/?env=dev&path=/authors/Vonnegut/books/Cats Cradle/reviews/`
3. Log in when prompted, if necessary.
4. Type JSON on the left, then hit `Option + Enter` to push it to Firestore. Collections must be arrays, docs must be objects/dicts.

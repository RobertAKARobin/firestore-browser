# Firestore Browser

1. Put your Firebase creds in files named `env.{environment_name}.json`, e.g. `env.dev.json`.
2.a. Go to `/?env={environment_name}&path={firestore_path}`, e.g. `/?env=dev&path=/authors/Vonnegut/books/Cats Cradle/reviews/`
2.b. Open your browser console to watch for errors.
3. Log in when prompted, if necessary.
4. The data at that path will be output on the right.
4. Type JSON input on the left, then hit `Option + Enter` to push it to Firestore. Collections must be arrays, docs must be objects/dicts.

## Notes:

- When you push data, it will completely overwrite whatever is at the current path.
- Each document in the output contains a property called `__firestore_id`, which unsurprisingly is the doc's Firestore ID. This property will be stripped from any docs that you push to Firestore.
- Output is saved to a global variable called `results`, which you can access in your browser console.
